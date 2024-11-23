## **Control Structures in JavaScript**

Control structures are constructs that dictate the flow of execution in a program based on conditions or repeated actions. JavaScript provides several control structures, such as conditional statements (`if`, `else`, `switch`) and loops (`for`, `while`, `do-while`, etc.).

---

## **1. Conditional Statements**

Conditional statements allow you to execute specific blocks of code based on a condition.

### **1.1 `if` Statement**

The `if` statement executes a block of code only if a specified condition evaluates to `true`.

**Syntax**:

```jsx
if (condition) {
    // Code to execute if the condition is true
}

```

**Example**:

```jsx
let age = 18;
if (age >= 18) {
    console.log("You are eligible to vote.");
}

```

### **1.2 `if-else` Statement**

The `if-else` statement provides an alternative block of code to execute if the condition is `false`.

**Syntax**:

```jsx
if (condition) {
    // Code to execute if the condition is true
} else {
    // Code to execute if the condition is false
}

```

**Example**:

```jsx
let age = 16;
if (age >= 18) {
    console.log("You are eligible to vote.");
} else {
    console.log("You are not eligible to vote.");
}

```

### **1.3 `if-else if` Ladder**

This structure is used to test multiple conditions.

**Syntax**:

```jsx
if (condition1) {
    // Code to execute if condition1 is true
} else if (condition2) {
    // Code to execute if condition2 is true
} else {
    // Code to execute if all conditions are false
}

```

**Example**:

```jsx
javascript
Copy code
let score = 85;
if (score >= 90) {
    console.log("Grade: A");
} else if (score >= 75) {
    console.log("Grade: B");
} else {
    console.log("Grade: C");
}

```

### **1.4 Ternary Operator**

A shorthand for `if-else`.

**Syntax**:

```jsx
javascript
Copy code
condition ? expressionIfTrue : expressionIfFalse;

```

**Example**:

```jsx
javascript
Copy code
let age = 20;
let result = (age >= 18) ? "Adult" : "Minor";
console.log(result);

```

---

### **1.5 `switch` Statement**

The `switch` statement tests a variable against multiple possible values and executes a block of code that matches.

**Syntax**:

```jsx
javascript
Copy code
switch (expression) {
    case value1:
        // Code to execute if expression === value1
        break;
    case value2:
        // Code to execute if expression === value2
        break;
    default:
        // Code to execute if no case matches
}

```

**Example**:

```jsx
javascript
Copy code
let day = 2;
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    default:
        console.log("Invalid day");
}

```

- **`break`**: Exits the `switch` block. Without it, execution continues to the next case.
- **`default`**: Executes if no cases match.

---

## **2. Loops**

Loops allow you to execute a block of code repeatedly based on a condition.

### **2.1 `for` Loop**

The `for` loop repeats a block of code a fixed number of times.

**Syntax**:

```jsx
javascript
Copy code
for (initialization; condition; increment/decrement) {
    // Code to execute in each iteration
}

```

**Example**:

```jsx
javascript
Copy code
for (let i = 1; i <= 5; i++) {
    console.log("Iteration:", i);
}

```

- **Initialization**: Runs once before the loop starts.
- **Condition**: Checked before each iteration; if `false`, the loop ends.
- **Increment/Decrement**: Updates the loop variable after each iteration.

---

### **2.2 `while` Loop**

The `while` loop repeats a block of code as long as the condition is `true`.

**Syntax**:

```jsx
javascript
Copy code
while (condition) {
    // Code to execute while the condition is true
}

```

**Example**:

```jsx
javascript
Copy code
let count = 1;
while (count <= 5) {
    console.log("Count:", count);
    count++;
}

```

---

### **2.3 `do-while` Loop**

The `do-while` loop is similar to `while`, but the code block executes at least once, even if the condition is initially `false`.

**Syntax**:

```jsx
javascript
Copy code
do {
    // Code to execute
} while (condition);

```

**Example**:

```jsx
javascript
Copy code
let num = 1;
do {
    console.log("Number:", num);
    num++;
} while (num <= 5);

```

---

### **2.4 `for-in` Loop**

The `for-in` loop is used to iterate over the properties of an object.

**Syntax**:

```jsx
javascript
Copy code
for (key in object) {
    // Code to execute for each property
}

```

**Example**:

```jsx
javascript
Copy code
let student = { name: "John", age: 20, grade: "A" };
for (let key in student) {
    console.log(key, ":", student[key]);
}

```

---

### **2.5 `for-of` Loop**

The `for-of` loop is used to iterate over iterable objects like arrays, strings, or NodeLists.

**Syntax**:

```jsx
javascript
Copy code
for (element of iterable) {
    // Code to execute for each element
}

```

**Example**:

```jsx
javascript
Copy code
let numbers = [10, 20, 30];
for (let num of numbers) {
    console.log(num);
}

```

---

## **3. Control Statements for Loops**

- **`break`**: Exits the loop immediately.
**Example**:
    
    ```jsx
    javascript
    Copy code
    for (let i = 1; i <= 5; i++) {
        if (i === 3) {
            break; // Exit the loop when i is 3
        }
        console.log(i);
    }
    
    ```
    
- **`continue`**: Skips the current iteration and moves to the next.
**Example**:
    
    ```jsx
    javascript
    Copy code
    for (let i = 1; i <= 5; i++) {
        if (i === 3) {
            continue; // Skip the iteration when i is 3
        }
        console.log(i);
    }
    
    ```
    

---

## **4. Combining Control Structures**

You can use conditional statements inside loops or vice versa.

**Example**:

```jsx
javascript
Copy code
for (let i = 1; i <= 10; i++) {
    if (i % 2 === 0) {
        console.log(i, "is even");
    } else {
        console.log(i, "is odd");
    }
}

```

---

### **Summary**

- Conditional statements (`if`, `else`, `switch`) decide the flow of execution based on conditions.
- Loops (`for`, `while`, `do-while`) repeat a block of code as long as conditions are met.
- Special loop control (`break`, `continue`) helps manage loop execution.
- JavaScript's control structures are powerful for building dynamic and interactive web applications.