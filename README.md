# MongoDB $inc Operator Error with String Value
This repository demonstrates an uncommon error encountered when using the MongoDB $inc operator.  The error arises from attempting to increment a field using a string value instead of a numerical value.

## Bug Description
The `$inc` operator in MongoDB is used to increment a numerical field by a specified value. Using a string value with `$inc` leads to an error because the operator expects a number.

## Solution
The solution involves using a numerical value for the increment.

## How to reproduce
1. Run MongoDB
2. Create a collection called 'myCollection'
3. Insert a document with an _id field and a field that you want to increment, for example:
```javascript
db.myCollection.insertOne({ _id: 1, field: 0 });
```
4. Run the incorrect code in the bug.js file, which will result in an error
5. Run the corrected code in the bugSolution.js file, which will correctly increment the field.
