# Suduko-game
This Sudoku Solver project is in Python. Talking about the
features of this system, this python application is designed
to solve number puzzles. You can use solver from the option to solve the puzzle if you want. Also, you can submit
your answer after completing the puzzle.

## Approach
The first approach is applying brute force to the problem. We can apply a backtracking algorithm by iterating over all the empty cells, beginning with the value 1 and checking it’s valid. We then move to the next empty cell, set that to 1 and check it’s valid. And so on. At any point we encounter an impossible solution (a cell with no valid values), we try the next value, and then the next. Should we exhaust all combinations in the current cell, we backtrack a loop, increment the previous cell value and begin again.
With such an approach, it’s not uncommon to backtrack all the way to start several times. To implement this approach we can use a simple loop and apply recursion (a function that calls itself with an altered or cut-down problem space) — the logic is only a few lines.
