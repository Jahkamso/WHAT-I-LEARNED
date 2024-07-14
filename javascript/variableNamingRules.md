Naming variable correctly is important because it makes your code more readable, understandable, and maintainable.

### Rules for Variable Names

1. Begin with a Letter, Underscore (_), or Dollar Sign ($) <br>

Example:
```js
var name;
var _name;
var $name;
```

2. Subsequent Characters Can Include Numbers:
<br>

Example:
```js
var name1;
var _name1;
var $name1;
```

3. Case-Sensitive: Variables are case sensitive which means `myVar` and `myvar` are considered as two totally different variables.
<br>

Example:
```js
var myVar;
var myvar;
```

4. No Reserved Words: Using reserved keywords like `let`, `class`, `function`, `return`, etc... will result in errors and cannot be used as a variable name.
<br>

Example:
```js
// Invalid
var let = 10;
var class = "myClass";
```

### Best Practices for Variable Names

1. Descriptive and Meaningful: Variable names should clearly describe their purpose or the data they hold.
<br>

Example:
```js
var firstName;
var totalPrice;
```

2. CamelCase Convention: Starting with a lowercase letter and capitalizing the first letter of each subsequent word.
<br>

Example:
```js
var userName;
var totalAmount;
```

3. Avoid Single-Letter Names: Avoid using single-letter names except for loop counters or variables with very short-lived scope.
<br>

Example:
```js
for (let i = 0; i < 10; i++) {
  // 'i' is acceptable here as a loop counter
}
```

4. Consistency: Be consistent with your naming conventions throughout your codebase.
<br>

Example:
```js
// If you start with camelCase, stick to it
var userAge;
var userAddress;
```

5. Avoid Abbreviations: Avoid abbreviations unless they are commonly understood.
<br>

Example:
```js
// Not recommended
var usrAddr;

// Better
var userAddress;
```

### Real-World Examples

Take for example you're developing a simple e-commerce website. These are some examples of good variable names:

```js
// User Information
var userName = "JohnDoe";
var userEmail = "john.doe@example.com";

// Shopping Cart
var cartItems = [];
var totalPrice = 0;

// Product Information
var productId = 12345;
var productName = "Wireless Mouse";
var productPrice = 29.99;
```

As you can see in the code above, it's very readable and clear to understand, which will make it easier for you to maintain the code.