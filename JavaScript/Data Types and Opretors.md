## **I. Data Types in JavaScript**

JavaScript is a dynamically typed language, meaning variables can hold values of any type without declaring the type explicitly. There are two main categories:

1. **Primitive Data Types**: Immutable, directly contain values.
2. **Non-Primitive (Reference) Data Types**: Mutable, store references to memory locations.

---

### **1. Primitive Data Types**

These are the basic building blocks of data in JavaScript.

1. **String**:
    - Represents textual data.
    - Strings are enclosed in single quotes (`'`), double quotes (`"`), or backticks (```).
    - Example:
        
        ```jsx
        let message = "Hello, World!";
        let name = 'Alice';
        let greeting = `Hi, ${name}`;
        
        ```
        
2. **Number**:
    - Represents both integers and floating-point numbers.
    - Special values: `Infinity`, `Infinity`, and `NaN` (Not-a-Number).
    - Example:
        
        ```jsx
        let age = 25; // Integer
        let price = 19.99; // Floating-point number
        let invalid = "abc" / 2; // NaN
        
        ```
        
3. **Boolean**:
    - Logical values: `true` or `false`.
    - Example:
        
        ```jsx
        let isActive = true;
        let hasPermission = false;
        
        ```
        
4. **Undefined**:
    - A variable declared but not assigned a value.
    - Example:
        
        ```jsx
        let user;
        console.log(user); // undefined
        
        ```
        
5. **Null**:
    - Represents the intentional absence of any value.
    - Example:
        
        ```jsx
        let emptyValue = null;
        
        ```
        
6. **Symbol** (introduced in ES6):
    - A unique, immutable identifier used in objects.
    - Example:
        
        ```jsx
        let id = Symbol("uniqueID");
        
        ```
        
7. **BigInt** (introduced in ES11):
    - Represents very large integers.
    - Example:
        
        ```jsx
        let bigNumber = 12345678901234567890n;
        
        ```
        

---

### **2. Non-Primitive Data Types**

These hold collections or complex entities.

1. **Object**:
    - A collection of key-value pairs.
    - Example:
        
        ```jsx
        let user = { name: "Alice", age: 25 };
        ```
        
2. **Array**:
    - An ordered collection of values.
    - Example:
        
        ```jsx
        let fruits = ["apple", "banana", "cherry"];
        ```
        
3. **Function**:
    - A reusable block of code.
    - Example:
        
        ```jsx
        function greet(name) {
          return `Hello, ${name}`;
        }
        ```
        
4. **Date**:
    - Used to handle dates and times.
    - Example:
        
        ```jsx
        let today = new Date();
        ```
        

---

## **II. JavaScript Operators**

Operators are used to perform operations on variables and values.

---

### **1. Arithmetic Operators**

Perform mathematical operations.

| Operator | Description | Example |
| --- | --- | --- |
| `+` | Addition | `5 + 3 = 8` |
| `-` | Subtraction | `5 - 3 = 2` |
| `*` | Multiplication | `5 * 3 = 15` |
| `/` | Division | `6 / 3 = 2` |
| `%` | Modulus (remainder) | `5 % 3 = 2` |
| `**` | Exponentiation | `2 ** 3 = 8` |

---

### **2. Assignment Operators**

Used to assign values to variables.

| Operator | Description | Example |
| --- | --- | --- |
| `=` | Assign | `x = 10` |
| `+=` | Add and assign | `x += 5` |
| `-=` | Subtract and assign | `x -= 2` |
| `*=` | Multiply and assign | `x *= 3` |
| `/=` | Divide and assign | `x /= 2` |

---

### **3. Comparison Operators**

Used to compare values and return a Boolean (`true` or `false`).

| Operator | Description | Example |
| --- | --- | --- |
| `==` | Equal to (type conversion) | `5 == "5"` → true |
| `===` | Strict equal (no conversion) | `5 === "5"` → false |
| `!=` | Not equal to | `5 != "5"` → false |
| `!==` | Strict not equal | `5 !== "5"` → true |
| `<` | Less than | `3 < 5` → true |
| `>` | Greater than | `5 > 3` → true |
| `<=` | Less than or equal to | `5 <= 5` → true |
| `>=` | Greater than or equal to | `5 >= 3` → true |

---

### **4. Logical Operators**

Used to combine multiple conditions.

| Operator | Description | Example |
| --- | --- | --- |
| `&&` | Logical AND | `true && false` → false |
| ` |  | ` |
| `!` | Logical NOT | `!true` → false |

---

### **5. String Operators**

Used to concatenate or manipulate strings.

| Operator | Description | Example |
| --- | --- | --- |
| `+` | Concatenation | `"Hello" + " World"` |

---

### **6. Ternary Operator**

A shorthand for `if-else`.

Syntax:

```jsx
javascript
Copy code
condition ? expr1 : expr2;

```

Example:

```jsx
javascript
Copy code
let age = 18;
let status = age >= 18 ? "Adult" : "Minor";
console.log(status); // Adult

```

---

### **7. Type Operators**

Used to check or convert types.

| Operator | Description | Example |
| --- | --- | --- |
| `typeof` | Returns type of a value | `typeof "hello"` → string |
| `instanceof` | Checks if an object is an instance of a class | `[] instanceof Array` → true |