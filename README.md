# MongoDB $inc Operator Error: Invalid Increment Value
This example demonstrates an incorrect usage of the `$inc` operator in a MongoDB update operation. The `$inc` operator is used to increment a numerical field in a document by a specified value. In this case, we're attempting to increment the "count" field by the string "1", which leads to an error.
The solution shows the correct way to use the `$inc` operator by providing a numerical value for the increment.
## Bug
The bug is in the usage of the `$inc` operator in the updateOne method. The `$inc` operator expects a numerical value to increment the field. Providing a string instead leads to an error.
## Solution
The correct way to use `$inc` is to provide the increment value as a number. This fixes the error and successfully updates the document.