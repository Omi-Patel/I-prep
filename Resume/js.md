# JavaScript Concepts and Interview Questions

## Table of Contents

1. [Introduction to JavaScript](#introduction-to-javascript)
2. [JavaScript Basics](#javascript-basics)
   - [Variables](#variables)
   - [Data Types](#data-types)
   - [Functions](#functions)
   - [Objects](#objects)
   - [Arrays](#arrays)
   - [Conditionals](#conditionals)
   - [Loops](#loops)
3. [Advanced JavaScript](#advanced-javascript)
   - [Hoisting](#hoisting)
   - [Closures](#closures)
   - [Scope](#scope)
   - [Prototypes and Inheritance](#prototypes-and-inheritance)
   - [Callbacks and Promises](#callbacks-and-promises)
   - [Async/Await](#asyncawait)
   - [Event Loop](#event-loop)
4. [Common JavaScript Functions](#common-javascript-functions)
5. [Important Interview Questions](#important-interview-questions)
   1. [What are JavaScript data types?](#what-are-javascript-data-types)
   2. [Explain `var`, `let`, and `const`.](#explain-var-let-and-const)
   3. [What is closure in JavaScript?](#what-is-closure-in-javascript)
   4. [What is event delegation?](#what-is-event-delegation)
   5. [Explain promises in JavaScript.](#explain-promises-in-javascript)
   6. [Explain event bubbling and event capturing.](#explain-event-bubbling-and-event-capturing)
   7. [What is a callback function?](#what-is-a-callback-function)
   8. [What is hoisting in JavaScript?](#what-is-hoisting-in-javascript)
   9. [What is `this` keyword?](#what-is-this-keyword)
   10. [What is the difference between `==` and `===` in JavaScript?](#what-is-the-difference-between-equality-operators-in-javascript)
   11. [What is prototype chain?](#what-is-prototype-chain)
   12. [What is the difference between synchronous and asynchronous programming?](#what-is-the-difference-between-synchronous-and-asynchronous-programming)

---

## 1. Introduction to JavaScript

JavaScript is a versatile, high-level programming language commonly used to create dynamic and interactive websites. It enables developers to build features such as animations, user interaction, and asynchronous behaviors.

Key features of JavaScript:

- Lightweight and interpreted language
- Event-driven and non-blocking
- Supports both object-oriented and functional programming paradigms
- Works on both the client-side and server-side (Node.js)

---

## 2. JavaScript Basics

### Variables

Variables in JavaScript are containers for storing data values. There are three ways to declare variables: `var`, `let`, and `const`.

```js
var name = "John"; // Function-scoped
let age = 25; // Block-scoped
const PI = 3.14; // Block-scoped and read-only
```

### Data Types

JavaScript provides several data types to hold different kinds of values:

- Primitive types: `String`, `Number`, `Boolean`, `Undefined`, `Null`, `Symbol`, `BigInt`
- Reference types: `Object`, `Array`, `Function`

### Functions

Functions are reusable blocks of code in JavaScript.

```js
function greet(name) {
  return "Hello " + name;
}
```

### Objects

Objects in JavaScript are collections of key-value pairs.

```js
const car = {
  make: "Toyota",
  model: "Camry",
  year: 2021,
};
```

### Arrays

Arrays in JavaScript are used to store multiple values in a single variable.

```js
let fruits = ["Apple", "Banana", "Mango"];
```

### Conditionals

Conditional statements help in decision making.

```js
if (age > 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

### Loops

Loops allow repeated execution of code.

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

---

## 3. Advanced JavaScript

### Hoisting

In JavaScript, variable and function declarations are moved to the top of their scope. This is called hoisting.

```js
console.log(x); // Undefined
var x = 5;
```

### Closures

A closure is created when a function retains access to variables from its outer scope, even after the outer function has returned.

```js
function outer() {
  let count = 0;
  return function inner() {
    count++;
    return count;
  };
}
let counter = outer();
```

### Scope

JavaScript has function scope and block scope. Variables declared with `var` are function-scoped, while `let` and `const` are block-scoped.

### Prototypes and Inheritance

In JavaScript, objects inherit properties and methods from their prototypes, enabling prototype-based inheritance.

```js
function Car(make) {
  this.make = make;
}
Car.prototype.start = function () {
  console.log(this.make + " is starting");
};
```

### Callbacks and Promises

Callbacks are functions passed as arguments to other functions and executed later. Promises provide a cleaner way to handle asynchronous operations.

```js
let promise = new Promise((resolve, reject) => {
  resolve("Success");
});
```

### Async/Await

`async` and `await` make it easier to work with promises.

```js
async function fetchData() {
  let response = await fetch("api/data");
  return response.json();
}
```

### Event Loop

JavaScript's event loop handles asynchronous operations, allowing non-blocking I/O.

```js
console.log("Start");
setTimeout(() => console.log("Delayed"), 1000);
console.log("End");
```

---

## 4. Common JavaScript Functions

1. `map()`: Transforms array elements.
2. `filter()`: Filters array elements based on a condition.
3. `reduce()`: Reduces array to a single value.
4. `forEach()`: Executes a function for each array element.
5. `find()`: Returns the first matching element in an array.

---

## 5. Important Interview Questions

### 1. What are JavaScript data types?

JavaScript has seven primitive data types: `String`, `Number`, `Boolean`, `Undefined`, `Null`, `Symbol`, and `BigInt`, and one reference type, `Object`.

### 2. Explain `var`, `let`, and `const`.

- `var`: Function-scoped, can be redeclared.
- `let`: Block-scoped, cannot be redeclared.
- `const`: Block-scoped, must be initialized at declaration and cannot be reassigned.

### 3. What is closure in JavaScript?

A closure is a function that retains access to its lexical scope, even when the function is executed outside that scope.

### 4. What is event delegation?

Event delegation is a technique where a single event listener is attached to a parent element to manage events for multiple child elements.

### 5. Explain promises in JavaScript.

Promises are used for handling asynchronous operations. They represent a value that may be available now, later, or never.

### 6. Explain event bubbling and event capturing.

Event bubbling is when an event starts from the innermost element and propagates outward. Event capturing is the reverse, where the event is captured from the outermost element and moves inward.

### 7. What is a callback function?

A callback is a function passed as an argument to another function and executed after some operation completes.

### 8. What is hoisting in JavaScript?

Hoisting is JavaScript's default behavior of moving declarations (but not initializations) to the top of the current scope.

### 9. What is `this` keyword?

`this` refers to the object from which a function is called.

### 10. What is the difference between `==` and `===` in JavaScript?

- `==`: Checks for value equality with type coercion.
- `===`: Checks for value and type equality without coercion.

### 11. What is prototype chain?

The prototype chain is the mechanism by which objects inherit properties and methods from their prototypes.

### 12. What is the difference between synchronous and asynchronous programming?

Synchronous programming executes one task at a time, blocking further execution. Asynchronous programming allows multiple tasks to run concurrently, using callbacks, promises, or `async/await`.
