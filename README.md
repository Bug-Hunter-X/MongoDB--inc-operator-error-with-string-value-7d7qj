# MongoDB $inc Operator Error with String Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The error occurs when using a string value instead of a numerical value for incrementing a field.

## Bug Description:
The code incorrectly uses a string ('1') instead of a number (1) with the `$inc` operator. This results in the counter field not being incremented correctly, potentially leading to data inconsistencies and unexpected program behavior.

## Solution:
The solution involves replacing the string value with a numerical value (1) to ensure correct increment operation.

## How to reproduce:
1.  Set up a MongoDB instance.
2.  Create a collection called `myCollection`.
3.  Insert a document with a field `counter` initialized to 0.
4.  Run the buggy code found in `bug.js`.
5.  Observe that the `counter` field is not incremented.
6.  Run the corrected code in `bugSolution.js`, which uses the numeric value.
7. Observe that the `counter` field is incremented correctly.
