# MaxSum
## Problem
You will have an orthogonal triangle input from a file and you need to find the maximum sum of the numbers according to given rules below;

1. You will start from the top and move downwards to an adjacent number as in below.
2. You are only allowed to walk downwards and diagonally.
3. You can only walk over NON PRIME NUMBERS.
4. You have to reach at the end of the pyramid as much as possible.
5. You have to treat your input as pyramid.

## Solution
1. Take the input file and convert it to a 2D array of ints
2. Traverse array for prime numbers and set them to 0
3. Calculate the maximum sum possible by comparing each value in the array with the value directly below or below and to the right of it, then adding the greater value of those values to it. If either of those two values are prime (prime numbers are set equal to 0), the value should be eliminated (set to 0) as it could not be walked over.
4. Print the maximum sum which is in the first column of the first row of the array.
