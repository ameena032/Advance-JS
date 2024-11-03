

# How to Check for Empty Arrays
Checking if an array is empty can be done with the `length` property.

### Example
```javascript
const isEmpty = arr => Array.isArray(arr) && arr.length === 0;
