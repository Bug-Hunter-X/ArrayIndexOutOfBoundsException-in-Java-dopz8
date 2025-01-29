# Java ArrayIndexOutOfBoundsException Bug

This repository demonstrates a common Java error: the `ArrayIndexOutOfBoundsException`. The `BuggyArray.java` file contains code that attempts to access an array element outside of its valid index range, leading to the exception. The `FixedArray.java` file shows the corrected code.

## How to Reproduce

1. Clone this repository.
2. Compile and run `BuggyArray.java`. Observe the exception.
3. Compile and run `FixedArray.java`. Observe the correct output.

## Solution

The bug is caused by the incorrect loop condition in `BuggyArray.java`. The loop should iterate from 0 up to (but not including) the length of the array.  The corrected code in `FixedArray.java` uses the condition `i < arr.length` to prevent the error.