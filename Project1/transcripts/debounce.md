
# Javascript Debounce Tutorial
Debouncing ensures that a function is only called after a certain amount of time has passed since it was last called.

### Example
```javascript
function debounce(func, delay) {
    let timeout;
    return function(...args) {
        clearTimeout(timeout);
        timeout = setTimeout(() => func.apply(this, args), delay);
    };
}
