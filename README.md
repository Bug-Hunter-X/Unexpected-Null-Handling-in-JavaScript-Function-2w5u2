# Unexpected Null Handling in JavaScript Function

This repository demonstrates a potential issue with null handling in JavaScript functions and shows a more robust solution.

## Bug Description

The `foo` function handles null values by simply returning 0.  While this prevents errors from occurring, it also might mask other potential problems.  The function doesn't indicate when null values are encountered; the caller has no way of knowing whether the returned 0 is the correct result or a result of the null value input.  Better error handling is needed.

## Solution

The improved solution uses a more robust error handling method, which allows the caller to understand why the function failed or if the returned value is indeed correct.  This will prevent unexpected behavior or masked errors.