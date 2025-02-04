# Unexpected NaN Result Due to Incorrect Undefined Handling

This repository demonstrates a common JavaScript error where undefined values are not handled correctly, resulting in NaN instead of the expected null value.  The bug is in the `foo` function, which attempts to perform arithmetic on potentially undefined parameters without proper checks.

## Bug Description
The `foo` function is designed to add two numbers. However, it incorrectly handles undefined parameters, leading to `NaN` (Not a Number) when one of the parameters is `undefined`. The solution implements a more robust check that handles both `null` and `undefined` values correctly.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` and run it.  You'll see the unexpected `NaN` output.
3. Open `bugSolution.js` to see the corrected version.