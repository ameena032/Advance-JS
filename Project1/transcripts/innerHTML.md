

# DO NOT use innerHTML
Using `innerHTML` can lead to security vulnerabilities. Use `textContent` or DOM methods instead.

### Example
```javascript
const element = document.createElement('div');
element.textContent = 'Safe content';
