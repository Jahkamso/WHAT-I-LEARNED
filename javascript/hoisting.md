Hoisting is JavaScript's default behavior of moving declarations to the top. It simply means variables can be used before it's declared.

A simple example of hoisting:

```js
console.log(x); // Output: undefined
var x = 5;
console.log(x); // Output: 5
```

Javascript moves the undeclared code `var x` to the top so it seems it's actually written like this:

```js
var x;
console.log(x); // Output: undefined
x = 5;
console.log(x); // Output: 5
```

**Functions:**

```js
sayHello(); // Output: Hello!
function sayHello() {
  console.log('Hello!');
}
```

In the example above, the function declaration `function sayHello() { ... }` is hoisted to the top of the scope, so you can call `sayHello()` before the actual declaration.

****

**Real-world Usecase:**

Imagine you're working on a web application, and you have a configuration or initialization function that needs to be executed before anything else. Thanks to hoisting, you can place your function call at the top of your script for better readability, knowing that the function declaration can come later in the code.

```js
initializeApp();

function initializeApp() {
  // Initialize your app here
  console.log('App initialized!');
}
```

> **NOTE:** 
> `let and const`: Variables declared with let and const are also hoisted, but they are not initialized. This means you cannot use them before the declaration. Attempting to do so will result in a ReferenceError.