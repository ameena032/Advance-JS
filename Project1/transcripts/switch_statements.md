
# STOP Using Switch Statements!
Switch statements can be less efficient. Use objects or functions instead.

### Example
```javascript
const actions = {
    START: () => console.log("Started"),
    STOP: () => console.log("Stopped")
};

const action = actions[command] || (() => console.log("Unknown command"));
action();
