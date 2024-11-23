## **JavaScript Syntax and Variables**

JavaScript syntax refers to the set of rules that define how JavaScript programs are written and interpreted. Variables are the fundamental building blocks of JavaScript, used to store and manage data.

---

## **I. JavaScript Syntax**

### **1. Case Sensitivity**

JavaScript is **case-sensitive**, meaning `variable` and `Variable` are treated as different identifiers.

### **2. Statements**

A **statement** is an instruction to perform a specific action. Statements are typically written on separate lines and terminated with a semicolon (`;`) (optional but recommended for clarity).

Example:

```jsx
let x = 5; // This is a statement
```

### **3. Code Blocks**

Statements grouped inside `{}` form a **code block**. Code blocks are used in structures like functions, loops, and conditionals.

Example:

```jsx
if (x > 0) {
    console.log("Positive number");
}

```

### **4. Comments**

Comments are ignored by the JavaScript engine and used for code documentation.

- **Single-line comment**: Starts with `//`
    
    ```jsx
    // This is a single-line comment
    
    ```
    
- **Multi-line comment**: Enclosed between `/*` and `/`
    
    ```jsx
    /* This is a
       multi-line comment */
    
    ```
    

### **5. JavaScript Keywords**

Keywords are reserved words used to perform specific tasks. Examples: `let`, `var`, `const`, `if`, `for`, `return`, etc.

---

### **II. JavaScript Variables**

Variables are used to store data values. You can declare variables using the `var`, `let`, or `const` keywords.

---

### **1. Declaring Variables**

- **`var`**: The original keyword for variable declaration.
    - Global or function-scoped.
    - Can be redeclared and reassigned.
    - Example:
        
        ```jsx
        var name = "Alice";
        name = "Bob"; // Reassignment
        var name = "Charlie"; // Redeclaration
        
        ```
        
- **`let`**: Introduced in ES6, it is block-scoped.
    - Cannot be redeclared in the same scope.
    - Example:
        
        ```jsx
        let age = 25;
        age = 30; // Reassignment allowed
        
        ```
        
- **`const`**: Block-scoped and used for constants.
    - Cannot be reassigned or redeclared.
    - Must be initialized at the time of declaration.
    - Example:
        
        ```jsx
        const PI = 3.14;
        // PI = 3.15; // Error
        
        ```
        

---

### **2. Variable Scope**

The scope of a variable determines where it can be accessed.

1. **Global Scope**:
    - Variables declared outside any function or block.
    - Example:
        
        ```jsx
        var globalVar = "I'm global";
        
        ```
        
2. **Function Scope**:
    - Variables declared inside a function are accessible only within that function.
    - Example:
        
        ```jsx
        function greet() {
            var message = "Hello!";
            console.log(message); // Accessible here
        }
        // console.log(message); // Error
        
        ```
        
3. **Block Scope**:
    - Variables declared with `let` or `const` inside `{}` are accessible only within that block.
    - Example:
        
        ```jsx
        if (true) {
            let blockVar = "Block scoped";
            console.log(blockVar); // Accessible here
        }
        // console.log(blockVar); // Error
        
        ```
        

---

### **3. Variable Hoisting**

- JavaScript moves variable declarations to the top of their scope at runtime.
- Applies to `var` but not `let` or `const`.

Example:

```jsx
console.log(a); // undefined
var a = 10;

```

For `let` or `const`:

```jsx
console.log(b); // Error: Cannot access 'b' before initialization
let b = 20;

```

---

### **III. Rules for Naming Variables**

1. Variable names must start with a letter, `_`, or `$`.
2. Cannot use reserved keywords as names (e.g., `let`, `function`).
3. Variable names are case-sensitive.

Examples:

```jsx
let firstName = "John"; // Valid
let _count = 42; // Valid
let $dollar = 100; // Valid
let 123name = "Invalid"; // Invalid

```

---

### **IV. Data Assignment and Initialization**

1. **Single Declaration**:
    
    ```jsx
    let age = 25;
    
    ```
    
2. **Multiple Declarations**:
    
    ```jsx
    let x = 10, y = 20, z = 30;
    
    ```
    
3. **Default Initialization**:
Variables declared without a value are `undefined` by default.
    
    ```jsx
    let unassigned;
    console.log(unassigned); // undefined
    
    ```
    

---

### **V. Examples of Variable Usage**

### **1. Using `var`**

```jsx
function greet() {
    var message = "Hello!";
    console.log(message); // Accessible inside function
}
greet();
// console.log(message); // Error

```

### **2. Using `let`**

```jsx
let age = 18;
if (true) {
    let age = 25; // Block-scoped
    console.log(age); // 25
}
console.log(age); // 18

```

### **3. Using `const`**

```jsx
const PI = 3.14;
console.log(PI);
// PI = 3.1415; // Error: Cannot reassign a const variable

```

### **4. Variable Hoisting**

```jsx
console.log(name); // undefined (var is hoisted)
var name = "Alice";

console.log(color); // Error (let is not hoisted)
let color = "blue";

```