# MongoDB $inc Operator with Non-Numeric Value
This repository demonstrates a common error encountered when using the MongoDB `$inc` operator with non-numeric values. The `$inc` operator is intended for incrementing numeric fields. Using it with a string or other non-numeric type results in a runtime error.
The `bug.js` file contains code that exemplifies this incorrect usage, and the `bugSolution.js` file provides a corrected version.
## Bug Description
Attempting to increment a field using `$inc` with a non-numeric value will throw an error. The error message will typically indicate a type mismatch or an invalid operation. 
## Solution
Ensure the field being incremented is of a numeric type and that the value used with `$inc` is also a number. Data validation before update operations is essential to prevent this type of error.