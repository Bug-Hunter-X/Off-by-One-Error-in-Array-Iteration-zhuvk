# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over arrays. The `BuggyArray.java` file contains code with the error, while `FixedArray.java` provides the corrected version.

The error occurs because the loop condition `i <= array.length` attempts to access an index that is out of bounds.  Arrays in Java are zero-indexed, so the valid indices range from 0 to `array.length - 1`.

The corrected code uses the condition `i < array.length`, ensuring that the loop iterates only within the valid index range.