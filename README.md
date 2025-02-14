# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript error related to closures and the `setTimeout` function within loops.

## Problem
The provided `bug.js` file contains a function that uses a `for` loop and `setTimeout` to log numbers from 0 to 9 with a 1-second delay.
Due to the nature of closures in JavaScript, it does not log the expected sequence of 0 through 9. Instead, it logs '10' ten times.

## Solution
The `bugSolution.js` file provides a corrected version that uses an immediately invoked function expression (IIFE) to create a new scope for each iteration of the loop, correctly capturing the value of `i` within each closure.