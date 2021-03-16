# Binairo Kata

Binairo is a logic puzzle game in which your goal is to fill a square grid (typically 12x12) with 1's and 0's.

The rules of the game are:

1. Fill all empty spaces with either a `0` or a `1`.
2. There should never be more than two of the same numbers next to each other (applies to rows and columns).
3. Every filled line and column should contain the same amount of numbers.

> A more advanced additional rule is than each line of numbers should be a unique combination. The same goes for columns.

## Exercise 1:

Create a function that takes some even amount of positions on the board and apply these rules:

1. If there are two equal numbers next to each other and there is an empty space or one or both sides, fill the empty space with the other number. So `.11.` should return `0110`.
2. If there are two equal numbers divided by an empty space, fill the empty space with the other number. So `0.0` should return `010`.
3. The function applies all rules until there is no more opportunity to fill empty spaces.

## Exercise 2:

1. Use rule number 3 to fill in even more empty spaces.
2. Make sure the number of spaces is even.

## Exercise 3:

1. Refactor the rule created with exercise 1.1 into a class named `PairJoiner`.
2. Refactor the rule created with exercise 1.2 into a class named `GapFiller`.
3. Refactor the rule created with exercise 2.1 into a class named `EqualOpportunity`.
4. Create a new class `BinairoSolver` that combines all rule classes for maximum 'autofill' effect.
5. Create a console app that:
  * sets up a pre-filled board of 12x12 spaces (you can use the example board below);
  * loops through all rows and columns and uses the `BinairoSolver` to solve the board as much as possible;
  * prints the board to the user.
6. Think about even more ways to fill empty spaces.

Example board:

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
