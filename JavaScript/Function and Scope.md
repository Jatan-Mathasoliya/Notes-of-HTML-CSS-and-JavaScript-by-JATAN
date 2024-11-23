## **Functions and Scope in JavaScript**

Functions are one of the core building blocks in JavaScript, allowing developers to organize code into reusable blocks. Scope defines the accessibility of variables and how they are tied to their context.

---

## **1. Functions**

### **1.1 What is a Function?**

A function is a block of reusable code designed to perform a specific task. It is executed when "called" or "invoked."

### **1.2 Why Use Functions?**

- **Reusability**: Write once, use multiple times.
- **Readability**: Break code into manageable parts.
- **Maintainability**: Easier to debug and update.

---

### **1.3 Defining and Calling Functions**

**Syntax**:

```jsx
function functionName(parameters) {
    // Code to execute
}

```

- **Parameters**: Inputs the function accepts.
- **Return Value**: The output the function produces, specified using the `return` keyword.

**Example**:

```jsx
function greet(name) {
    return `Hello, ${name}!`;
}

console.log(greet("Alice")); // Output: Hello, Alice!

```

---

### **1.4 Types of Functions**

### **1.4.1 Named Functions**

A function declared with a name.

**Example**:

```jsx
function add(a, b) {
    return a + b;
}

console.log(add(5, 3)); // Output: 8

```

### **1.4.2 Anonymous Functions**

Functions without a name, often assigned to variables or used as arguments.

**Example**:

```jsx
const subtract = function(a, b) {
    return a - b;
};

console.log(subtract(10, 5)); // Output: 5

```

### **1.4.3 Arrow Functions**

A concise way to write functions using the `=>` syntax.

**Syntax**:

```jsx
const functionName = (parameters) => {
    // Code to execute
};

```

**Example**:

```jsx
const multiply = (a, b) => a * b;
console.log(multiply(4, 5)); // Output: 20

```

---

### **1.5 Function Parameters and Arguments**

### **1.5.1 Default Parameters**

Provide default values for parameters when arguments are not supplied.

**Example**:

```jsx
function greet(name = "Guest") {
    return `Hello, ${name}!`;
}

console.log(greet()); // Output: Hello, Guest!
console.log(greet("Alice")); // Output: Hello, Alice!

```

### **1.5.2 Rest Parameters**

Gather all remaining arguments into a single array.

**Syntax**:

```jsx
function functionName(...restParameters) {
    // Code to execute
}

```

**Example**:

```jsx
function sum(...numbers) {
    return numbers.reduce((acc, num) => acc + num, 0);
}

console.log(sum(1, 2, 3, 4)); // Output: 10

```

---

### **1.6 Returning Values**

A function can return a value using the `return` statement.

**Example**:

```jsx
function square(num) {
    return num * num;
}

console.log(square(5)); // Output: 25

```

---

### **2. Scope**

Scope determines where variables can be accessed or modified in your code.

### **2.1 Types of Scope**

### **2.1.1 Global Scope**

Variables declared outside of any function or block have global scope and are accessible anywhere in the code.

**Example**:

```jsx
let globalVar = "I am global";

function showGlobalVar() {
    console.log(globalVar); // Accessible
}

showGlobalVar(); // Output: I am global

```

### **2.1.2 Function Scope**

Variables declared inside a function are accessible only within that function.

**Example**:

```jsx
function demoFunctionScope() {
    let localVar = "I am local";
    console.log(localVar); // Accessible
}

demoFunctionScope();
// console.log(localVar); // Error: localVar is not defined

```

### **2.1.3 Block Scope**

Variables declared with `let` or `const` inside a block (`{}`) are accessible only within that block.

**Example**:

```jsx
if (true) {
    let blockVar = "I am block-scoped";
    console.log(blockVar); // Accessible
}
// console.log(blockVar); // Error: blockVar is not defined

```

---

### **2.2 Variable Declarations and Scope**

### **`var` (Function Scoped)**

- Declared variables are hoisted to the top of their scope.
- Can be accessed before declaration (undefined).

**Example**:

```jsx
console.log(x); // Output: undefined
var x = 5;
console.log(x); // Output: 5

```

### **`let` and `const` (Block Scoped)**

- Not hoisted to the same extent as `var`.
- Cannot be accessed before declaration (Temporal Dead Zone).

**Example**:

```jsx
// console.log(y); // Error: Cannot access 'y' before initialization
let y = 10;
console.log(y); // Output: 10

```

---

### **3. Closures**

A closure is a function that "remembers" the variables from its outer scope, even after the outer function has finished executing.

**Example**:

```jsx
function outer() {
    let outerVar = "Outer";

    return function inner() {
        console.log(outerVar);
    };
}

const closureFunction = outer();
closureFunction(); // Output: Outer

```

---

### **4. Hoisting**

JavaScript hoists declarations to the top of their scope during the compilation phase.

**Example**:

```jsx
console.log(a); // Output: undefined
var a = 10;

// With let or const
// console.log(b); // Error: Cannot access 'b' before initialization
let b = 20;

```