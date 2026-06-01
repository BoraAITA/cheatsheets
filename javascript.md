# 🟨 JavaScript Cheatsheet (ES6+)

## Variables

```javascript
const constant = 10;        // Constant value
let variable = 20;          // Mutable value
// var oldWay = 30;         // Don't use!
```

## Functions

```javascript
// Arrow function
const hello = (name) => `Hello ${name}!`;

// Default parameter
const greet = (name = "World") => `Hello ${name}!`;

// Rest parameter
const sum = (...numbers) => numbers.reduce((a, b) => a + b, 0);
```

## Destructuring

```javascript
// Array
const [first, second] = [1, 2, 3];

// Object
const { name, age } = { name: "Ali", age: 25, city: "Istanbul" };

// Nested
const { address: { city } } = { address: { city: "Ankara" } };
```

## Array Methods

```javascript
const numbers = [1, 2, 3, 4, 5];

numbers.map(x => x * 2);        // [2, 4, 6, 8, 10]
numbers.filter(x => x > 3);     // [4, 5]
numbers.reduce((a, b) => a + b); // 15
numbers.find(x => x > 3);       // 4
numbers.some(x => x > 3);       // true
numbers.every(x => x > 0);      // true
```

## Async/Await

```javascript
const fetchData = async () => {
  try {
    const response = await fetch("https://api.example.com/data");
    const data = await response.json();
    return data;
  } catch (error) {
    console.error("Error:", error);
  }
};
```

## Spread & Rest

```javascript
// Spread
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5]; // [1, 2, 3, 4, 5]

const obj1 = { a: 1, b: 2 };
const obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }
```
