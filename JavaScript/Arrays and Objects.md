## **Arrays and Objects in JavaScript**

Arrays and Objects are fundamental data structures in JavaScript, allowing developers to store, organize, and manipulate collections of data.

---

## **1. Arrays in JavaScript**

An array is a collection of values stored in a single variable. Each value, called an *element*, is identified by an index starting from `0`.

### **1.1 Creating Arrays**

### **1.1.1 Using Array Literals**

The simplest and most common way to create an array.

**Example**:

```jsx
let fruits = ["Apple", "Banana", "Cherry"];
console.log(fruits); // Output: ["Apple", "Banana", "Cherry"]

```

### **1.1.2 Using the `Array` Constructor**

Another way to create arrays.

**Example**:

```jsx
let numbers = new Array(10); // Creates an empty array with length 10
let colors = new Array("Red", "Blue", "Green"); // Creates an array with elements
console.log(numbers.length); // Output: 10
console.log(colors); // Output: ["Red", "Blue", "Green"]

```

---

### **1.2 Accessing Array Elements**

Use the **index** to access array elements.

**Example**:

```jsx
let cities = ["New York", "London", "Tokyo"];
console.log(cities[0]); // Output: "New York"
console.log(cities[2]); // Output: "Tokyo"

```

---

### **1.3 Modifying Arrays**

Modify elements by assigning new values to a specific index.

**Example**:

```jsx
let animals = ["Dog", "Cat", "Bird"];
animals[1] = "Elephant"; // Replace "Cat" with "Elephant"
console.log(animals); // Output: ["Dog", "Elephant", "Bird"]

```

---

### **1.4 Array Properties**

### **1.4.1 `length` Property**

Returns the number of elements in an array.

**Example**:

```jsx
let cars = ["Toyota", "Ford", "BMW"];
console.log(cars.length); // Output: 3

```

---

### **1.5 Array Methods**

### **1.5.1 Adding/Removing Elements**

- **`push()`**: Add to the end.
- **`pop()`**: Remove from the end.
- **`unshift()`**: Add to the beginning.
- **`shift()`**: Remove from the beginning.

**Example**:

```jsx
let numbers = [1, 2, 3];
numbers.push(4); // Add 4 to the end
console.log(numbers); // Output: [1, 2, 3, 4]

numbers.pop(); // Remove last element
console.log(numbers); // Output: [1, 2, 3]

```

### **1.5.2 Iterating Over Arrays**

- **`for` Loop**:

```jsx
let fruits = ["Apple", "Banana", "Cherry"];
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}

```

- **`forEach()`**:

```jsx
fruits.forEach((fruit) => console.log(fruit));

```

### **1.5.3 Other Common Methods**

- **`slice()`**: Extract a portion of an array.
- **`splice()`**: Add/remove elements in the middle.
- **`join()`**: Combine elements into a string.
- **`map()`**: Apply a function to each element.

**Example**:

```jsx
let numbers = [1, 2, 3, 4];
let squared = numbers.map((num) => num * num);
console.log(squared); // Output: [1, 4, 9, 16]

```

Arrays and Objects are fundamental data structures in JavaScript, allowing developers to store, organize, and manipulate collections of data.

---

## **1. Arrays in JavaScript**

An array is a collection of values stored in a single variable. Each value, called an *element*, is identified by an index starting from `0`.

### **1.1 Creating Arrays**

### **1.1.1 Using Array Literals**

The simplest and most common way to create an array.

**Example**:

```jsx
let fruits = ["Apple", "Banana", "Cherry"];
console.log(fruits); // Output: ["Apple", "Banana", "Cherry"]

```

### **1.1.2 Using the `Array` Constructor**

Another way to create arrays.

**Example**:

```jsx
let numbers = new Array(10); // Creates an empty array with length 10
let colors = new Array("Red", "Blue", "Green"); // Creates an array with elements
console.log(numbers.length); // Output: 10
console.log(colors); // Output: ["Red", "Blue", "Green"]

```

---

### **1.2 Accessing Array Elements**

Use the **index** to access array elements.

**Example**:

```jsx
let cities = ["New York", "London", "Tokyo"];
console.log(cities[0]); // Output: "New York"
console.log(cities[2]); // Output: "Tokyo"

```

---

### **1.3 Modifying Arrays**

Modify elements by assigning new values to a specific index.

**Example**:

```jsx
animals = ["Dog", "Cat", "Bird"];
animals[1] = "Elephant"; // Replace "Cat" with "Elephant"
console.log(animals); // Output: ["Dog", "Elephant", "Bird"]

```

---

### **1.4 Array Properties**

### **1.4.1 `length` Property**

Returns the number of elements in an array.

**Example**:

```jsx
let cars = ["Toyota", "Ford", "BMW"];
console.log(cars.length); // Output: 3

```

---

### **1.5 Array Methods**

### **1.5.1 Adding/Removing Elements**

- **`push()`**: Add to the end.
- **`pop()`**: Remove from the end.
- **`unshift()`**: Add to the beginning.
- **`shift()`**: Remove from the beginning.

**Example**:

```jsx
let numbers = [1, 2, 3];
numbers.push(4); // Add 4 to the end
console.log(numbers); // Output: [1, 2, 3, 4]

numbers.pop(); // Remove last element
console.log(numbers); // Output: [1, 2, 3]

```

### **1.5.2 Iterating Over Arrays**

- **`for` Loop**:

```jsx
let fruits = ["Apple", "Banana", "Cherry"];
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}

```

- **`forEach()`**:

```jsx
fruits.forEach((fruit) => console.log(fruit));

```

### **1.5.3 Other Common Methods**

- **`slice()`**: Extract a portion of an array.
- **`splice()`**: Add/remove elements in the middle.
- **`join()`**: Combine elements into a string.
- **`map()`**: Apply a function to each element.

**Example**:

```jsx
let numbers = [1, 2, 3, 4];
let squared = numbers.map((num) => num * num);
console.log(squared); // Output: [1, 4, 9, 16]

```

### **1. `slice()` Example**

The **`slice()`** method extracts a portion of an array without modifying the original array.

```jsx
let fruits = ["Apple", "Banana", "Cherry", "Date", "Elderberry"];

// Extract a portion of the array
let slicedFruits = fruits.slice(1, 4); // Extracts elements from index 1 to 3 (4 is excluded)
console.log(slicedFruits); // Output: ["Banana", "Cherry", "Date"]

// Original array remains unchanged
console.log(fruits); // Output: ["Apple", "Banana", "Cherry", "Date", "Elderberry"]

```

---

### **2. `splice()` Example**

The **`splice()`** method adds or removes elements in an array and modifies the original array.

```jsx
let numbers = [1, 2, 3, 4, 5];

// Removing elements
let removed = numbers.splice(1, 2); // Removes 2 elements starting from index 1
console.log(removed); // Output: [2, 3]
console.log(numbers); // Output: [1, 4, 5]

// Adding elements
numbers.splice(2, 0, 6, 7); // Adds 6 and 7 at index 2
console.log(numbers); // Output: [1, 4, 6, 7, 5]

// Replacing elements
numbers.splice(1, 2, 8, 9); // Replaces 2 elements starting at index 1 with 8 and 9
console.log(numbers); // Output: [1, 8, 9, 7, 5]

```

---

### **3. `join()` Example**

The **`join()`** method combines all elements of an array into a string, separated by a specified delimiter.

```jsx
let words = ["Hello", "world", "welcome", "to", "JavaScript"];

// Combine with spaces
let sentence = words.join(" ");
console.log(sentence); // Output: "Hello world welcome to JavaScript"

// Combine with dashes
let hyphenated = words.join("-");
console.log(hyphenated); // Output: "Hello-world-welcome-to-JavaScript"

// Combine without a delimiter
let concatenated = words.join("");
console.log(concatenated); // Output: "HelloworldwelcometoJavaScript"

```

---

### Key Points:

1. **`slice()`**:
    - Non-destructive (does not modify the original array).
    - Extracts a range of elements.
2. **`splice()`**:
    - Destructive (modifies the original array).
    - Can remove, add, or replace elements.
3. **`join()`**:
    - Converts an array into a string.
    - Allows specifying a delimiter for joining.


# **Objects in JavaScript**

## **What Are Objects?**

In JavaScript, objects are collections of key-value pairs. They are one of the fundamental data types used to store and manipulate data in a structured form. An object can contain properties (data) and methods (functions).

---

### **Creating Objects**

### **1. Using Object Literals**

The most common way to create an object is using curly braces `{}`.

```jsx
let person = {
  name: "John",         // Property: Key-value pair
  age: 30,
  greet: function () {  // Method: A function as a value
    return `Hello, my name is ${this.name}`;
  }
};

console.log(person.name);    // Access property: Output: John
console.log(person.greet()); // Call method: Output: Hello, my name is John

```

---

### **2. Using the `new Object()` Constructor**

Another way to create objects is with the `Object()` constructor.

```jsx
let car = new Object();
car.brand = "Toyota";
car.model = "Corolla";
car.start = function () {
  return `${this.brand} ${this.model} is starting.`;
};

console.log(car.brand);  // Output: Toyota
console.log(car.start()); // Output: Toyota Corolla is starting.

```

---

### **3. Using Object.create()**

This method creates a new object using a specified prototype object.

```jsx
let prototypeCar = {
  type: "Sedan",
  drive: function () {
    return "Driving a " + this.type;
  }
};

let myCar = Object.create(prototypeCar);
myCar.type = "Hatchback";

console.log(myCar.drive()); // Output: Driving a Hatchback

```

---

### **Accessing and Modifying Object Properties**

### **1. Dot Notation**

Access properties using a dot (`.`).

```jsx
console.log(person.name); // Output: John
person.age = 35;          // Modify property
console.log(person.age);  // Output: 35

```

### **2. Bracket Notation**

Useful when the key is dynamic or not a valid identifier.

```jsx
let key = "name";
console.log(person[key]); // Output: John

person["country"] = "USA";  // Add a new property
console.log(person.country); // Output: USA

```

---

### **Deleting Properties**

The `delete` operator removes a property from an object.

```jsx
delete person.age;
console.log(person.age); // Output: undefined

```

---

### **Checking Properties**

### **1. Using the `in` Operator**

Checks if a property exists in the object.

```jsx
console.log("name" in person); // Output: true
console.log("age" in person);  // Output: false (if deleted)

```

### **2. Using `hasOwnProperty()`**

Checks if the property exists directly on the object (not inherited).

```jsx
console.log(person.hasOwnProperty("name")); // Output: true

```

---

### **Iterating Over Properties**

### **1. Using `for...in` Loop**

Iterates over all enumerable properties.

```jsx
for (let key in person) {
  console.log(`${key}: ${person[key]}`);
}
// Output:
// name: John
// country: USA

```

### **2. Using `Object.keys()`**

Gets an array of the object’s own property keys.

```jsx
let keys = Object.keys(person);
console.log(keys); // Output: ["name", "country"]

```

### **3. Using `Object.values()`**

Gets an array of the object’s own property values.

```jsx
let values = Object.values(person);
console.log(values); // Output: ["John", "USA"]

```

---

### **Advanced Features of Objects**

### **1. Nested Objects**

An object can have properties that are also objects.

```jsx
let student = {
  name: "Alice",
  grades: {
    math: 90,
    science: 85
  },
  getMathGrade: function () {
    return this.grades.math;
  }
};

console.log(student.grades.math); // Output: 90
console.log(student.getMathGrade()); // Output: 90

```

---

### **2. Object Destructuring**

Allows you to extract properties from an object into variables.

```jsx
let { name, country } = person;
console.log(name);    // Output: John
console.log(country); // Output: USA

```

---

### **3. Object Spread and Rest Operators**

**Spread Operator**: Copies properties from one object to another.

```jsx
let details = { ...person, job: "Developer" };
console.log(details);
// Output: { name: "John", country: "USA", job: "Developer" }

```

**Rest Operator**: Groups remaining properties into a new object.

```jsx
let { name, ...rest } = person;
console.log(rest); // Output: { country: "USA" }

```

---

### **Object Methods**

### **1. Object.freeze()**

Prevents modification of existing properties and addition of new properties.

```jsx
let frozenObj = Object.freeze({ prop: "value" });
frozenObj.prop = "newValue"; // No effect
console.log(frozenObj.prop); // Output: value

```

### **2. Object.seal()**

Allows modifying existing properties but prevents adding new ones.

```jsx
let sealedObj = Object.seal({ prop: "value" });
sealedObj.newProp = "newValue"; // Not allowed
sealedObj.prop = "newValue";    // Allowed
console.log(sealedObj); // Output: { prop: "newValue" }

```

---

### **Use Cases of Objects**

1. **Representing Real-World Entities**:
    - A `user` object can represent user data in an application.
2. **Data Storage**:
    - Objects are often used to group related data.
3. **Dynamic Data Structures**:
    - Objects allow the addition and removal of properties during runtime.
4. **API Responses**:
    - JSON data, commonly used in APIs, is based on object structure.

---

### **Key Takeaways**

1. Objects are versatile and allow for structured data representation.
2. You can add, modify, and delete properties dynamically.
3. Methods like `Object.keys()`, `Object.values()`, and `Object.entries()` provide efficient ways to interact with object data.
4. Advanced features like destructuring and spread/rest operators make working with objects more concise and readable.

By understanding objects in depth, you can effectively model and manipulate complex data in JavaScript!