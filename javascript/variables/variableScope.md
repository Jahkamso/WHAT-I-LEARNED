# What are Variable Scopes?

Variable scopes refers to how accessible variables are in your project.

There are 3 main scopes:

- Global
- Function
- Block scope

### Global Scope
These are variable names that aren't in a function or block scope, and can be accessed from anywhere.

Example:
```js
var globalVar = "I'm global!";

function displayGlobalVar() {
  console.log(globalVar); // Accessible here
}

displayGlobalVar(); // Output: I'm global!
console.log(globalVar); // Accessible here too
```

### Function Scope
These are variables that can only be accessed and used inside of the function it was declared in.

Example:
```js
function showMessage() {
  var message = "Hello, world!";
  console.log(message); // Accessible here
}

showMessage(); // Output: Hello, world!
console.log(message); // Error: message is not defined
```

### Block scope
Variables declare within a block of code with curly braces {} are block scopes and can't be accessed anywhere else.

Example:

```js
if (true) {
  let blockVar = "I'm block-scoped!";
  console.log(blockVar); // Accessible here
}

console.log(blockVar); // Error: blockVar is not defined
```