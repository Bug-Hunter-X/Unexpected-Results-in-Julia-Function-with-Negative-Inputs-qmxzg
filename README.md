# Julia Function Bug: Unexpected Results with Negative Inputs

This repository demonstrates a common bug in Julia involving unexpected results from a function when dealing with negative inputs. The issue arises from the order of operations and how negative numbers are handled within conditional statements.

## Bug Description
The function `myfunction` is designed to square the input if it's positive, return 0 if it's 0, and return the negative of the square if it's negative. However, due to operator precedence, the function produces incorrect results for negative inputs.

## Solution
The solution involves using parentheses to explicitly control the order of operations, ensuring that the negation happens before the squaring operation for negative inputs.