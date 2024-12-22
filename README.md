# Unexpected String Concatenation in JavaScript

This example demonstrates a common JavaScript error caused by its loose typing system. When adding a number and a string, JavaScript performs string concatenation instead of numerical addition.

## Bug

The `myFunction` adds two values, a number and a string.  Because JavaScript doesn't enforce strict type checking, it concatenates the string '5' to the number 5, resulting in the string '55'.

## Solution

The solution involves explicitly converting the string to a number using `parseInt()` or `Number()` before performing the addition to ensure a numerical result.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory containing `bug.js`.
3. Run `node bug.js` in your terminal.  You'll see the unexpected output.
4. Then run `node bugSolution.js` to see the corrected output.