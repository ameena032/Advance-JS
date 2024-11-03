# How to Curry Functions
### Example
```javascript
function curry(fn) {
    return function curried(...args) {
        if (args.length >= fn.length) {
            return fn(...args);
        }
        return function(...args2) {
            return curried(...args, ...args2);
        };
    };
}