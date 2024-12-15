# JavaScript Function Bug: Unexpected NaN Result

This repository demonstrates a common JavaScript bug related to unexpected NaN (Not a Number) results. The `foo` function intends to add two numbers, handling null values gracefully. However, it fails to handle the case where one of the inputs is NaN.  The bug and its solution are provided in separate JavaScript files.

## Bug Description

The `foo` function correctly handles null inputs, returning 0. However, if either `a` or `b` is `NaN`, the function returns `NaN` instead of 0, as would be expected in most practical situations. 

## Solution

The solution provided in `bugSolution.js` adds a check for `isNaN()` to address this edge case.  If either `a` or `b` is `NaN`, the function now returns 0, providing more robust and expected behavior. 