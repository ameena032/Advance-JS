

# Memoization and How to Memoize
Memoization is an optimization technique to speed up function calls by caching results.

### Example
```javascript
const memoize = (fn) => {
    const cache = {};
    return function(...args) {
        const key = JSON.stringify(args);
        if (!(key in cache)) {
            cache[key] = fn(...args);
        }
        return cache[key];
    };
};
