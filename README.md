# Sudoku-solver

## Description
The **Sudoku Solver** is a Python program that solves a 9x9 Sudoku puzzle. It takes an incomplete Sudoku grid as input, fills in the missing numbers, and outputs the completed grid. The solver uses a **backtracking algorithm** to efficiently find the solution by trying all possible values and reverting if a conflict arises.


## Features
- Accepts a 9x9 Sudoku grid with empty cells represented as `0`.
- Solves the puzzle using a **recursive backtracking algorithm**.
- Validates moves to ensure the solution follows Sudoku rules.
- Prints the solved Sudoku grid in a user-friendly format.


## Requirements
- Python 3.6 or later.


## How to Run
1. Clone or download the repository containing the `sudoku_solver.py` file.
2. Open a terminal or command prompt and navigate to the folder containing the script.
3. Run the script:
   ```bash
   python sudoku_solver.py
   ```
4. The program will solve the Sudoku puzzle provided in the code and display the solution in the terminal.

---

## Input Format
The input is a 9x9 grid represented as a 2D Python list. Empty cells are represented with `0`.

Example Input:
```python
sudoku_grid = [
    [5, 3, 0, 0, 7, 0, 0, 0, 0],
    [6, 0, 0, 1, 9, 5, 0, 0, 0],
    [0, 9, 8, 0, 0, 0, 0, 6, 0],
    [8, 0, 0, 0, 6, 0, 0, 0, 3],
    [4, 0, 0, 8, 0, 3, 0, 0, 1],
    [7, 0, 0, 0, 2, 0, 0, 0, 6],
    [0, 6, 0, 0, 0, 0, 2, 8, 0],
    [0, 0, 0, 4, 1, 9, 0, 0, 5],
    [0, 0, 0, 0, 8, 0, 0, 7, 9]
]
```

---

## Output Format
The solved Sudoku grid is printed in the terminal.

Example Output:
```
Solved Sudoku:
5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
```

---

## How It Works
1. The program uses a **backtracking algorithm** to recursively solve the puzzle.
2. It iterates through the grid to find empty cells (`0`).
3. For each empty cell, it tries placing a number (1-9) and checks if it’s valid:
   - The number must not exist in the same row, column, or 3x3 sub-grid.
4. If valid, it places the number and continues solving the remaining grid.
5. If a conflict occurs, it backtracks by removing the number and trying the next possible value.

---

## Limitations
- Only supports 9x9 Sudoku puzzles.
- Assumes the input grid is well-formed and solvable.

---

## License
This project is open-source and free to use. Feel free to modify or extend it as needed.

