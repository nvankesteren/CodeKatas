# Binairo Solver

Binairo is a logic puzzle game in which your goal is to fill a square grid (typically 12x12) with 1's and 0's. You can try it out at https://www.puzzle-binairo.com/ (in the options you can swap out white/black circles with 0's and 1's).

The rules of the game are:

1. Fill all empty spaces with either a `0` or a `1`.
2. There should never be more than two of the same numbers next to each other (applies to rows and columns).
3. Each row and column should contain the same amount of 0's and 1's.
4. Each row should have a unique combination of numbers. The same goes for columns.

> Do the exercises one at a time. Do *not* start with a board.

## Exercise 1

Create a class `BinairoSolver` with a function `string Solve(string)` that takes one line from the board as an input and tries to fill in the empty spaces as much as possible.

1. If there are two equal numbers next to each other and there is an empty space or one or both sides, fill the empty space with the other number. So `.11.` (where dots equal empty spaces) should return `0110`.
2. If there are two equal numbers divided by an empty space, fill the empty space with the other number. So `0.0` should return `010`.
3. If one of the numbers has reached its maximum for the line, fill the remaining empty spaces with the other number. So `..1011` should return `001011`.

## Exercise 2 

1. Make sure all the actions from exercise 1 repeat themselves until no other empty spaces can be filled.
2. Throw clear exceptions when invalid input is given, like an uneven number of positions, invalid position values (other than `0`, `1` or `.`), etc.

## Exercise 3

1. Create a new class `Game` that sets up a board (you can use one of the examples below).
2. Use the BinairoSolver with each row and column until no more empty space can be filled; avoid infinite loops.
3. Make sure the output of the BinairoSolver is written back to appropriate row or column on the board.
4. Have the ability to print the board.

Example boards:

(easy)
| | | | | | |
|-|-|-|-|-|-|
| | | |0| | |
| | | | | |1|
| | | |0| | |
| |1|1| | | |
|0| | | |0| |
| | |1| | | |

(hard)
| | | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|-|
| | | | | | | | |1| |1| |
| | |0| | | | | |1|1| | |
| | | | | |1|1| | | | |0|
| | |1|1| |0| | | | | |0|
| |0| | | | | |0| | | | |
| | | | |1| | | | | |1|0|
|1|1| | | | | |0| | |1| |
|.| | | | | | | | | | ||
|1| | | | |1| | | |1| |0|
| | |1| | | | | | |1| | |
| |0| | | | | | |0| | | |
|0| | | |1| | |1| | | | |
