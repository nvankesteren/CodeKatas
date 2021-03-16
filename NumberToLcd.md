# Number To LCD

Write a program that displays LCD style numbers. You can safely ignore invalid input and negative numbers.

> !!! Note: Please do NOT read ahead to other parts before completing the current part. Part of the purpose of this kata is to make you practice refactoring and adapting to changing requirements.

## Part 1

Write a program that given a digit, converts it into a LCD style digit using the following format:
```
   _  _     _  _  _  _  _  _ 
 | _| _||_||_ |_   ||_||_|| |  
 ||_  _|  | _||_|  ||_| _||_| 
 ```
(each digit is 3 lines high, starting with underscores for the numbers that need it)

## Part 2

Modify the program that the input can be a number (with an arbitrary number of digits), converts it into an LCD style number.

## Part 3

Change your program to support variable width or height of the digits. For example for width = 3 and height = 2 the digit 2 will be:
```
 ___
    |
 ___|
|
|___
```
