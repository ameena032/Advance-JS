
# Composition vs Inheritance
Composition is a design principle where classes achieve functionality by containing instances of other classes.

### Example
```javascript
class Engine {
    start() {
        console.log("Engine started");
    }
}

class Car {
    constructor() {
        this.engine = new Engine();
    }

    start() {
        this.engine.start();
    }
}
