# OOP Sudoku

A Sudoku puzzle generator and solver written in Python, built around clean object-oriented design. The `Board` class (fully documented with docstrings) generates valid puzzles, removes cells to set easy/medium/hard difficulty, and solves boards with a backtracking algorithm. A pygame GUI lets you play the generated puzzles interactively in a window titled "Sudoku by Owen."

## Features

- `Board` class encapsulating grid state, difficulty, generation, and solving
- Puzzle generation with difficulty levels controlled by empty-cell counts
- Backtracking solver that can solve any generated board and reveal the solution
- Board validation helpers (`is_solved`, `get_valid_numbers`, row/column/box accessors)
- Interactive pygame GUI: click cells and enter numbers on a rendered 9×9 grid
- NumPy-documented docstrings on the public API

## Tech Stack

- Python 3
- pygame (GUI)
- numpy (board math)

## Getting Started

1. Install Python 3.
2. Install dependencies:
   ```
   pip install pygame numpy
   ```
3. Run the game:
   ```
   python sudoku_gui.py
   ```

## Project Structure

```
OOP_Sudoku/
├── sudoku_solver_gen3.py  # Board class: generation, solving, validation
└── sudoku_gui.py          # pygame interface (540×600 window)
```

## Status / Notes

- The solver and generator are complete; the GUI is a functional playable prototype.
- Difficulty is tuned via empty-cell counts per level rather than a formal difficulty rating.
