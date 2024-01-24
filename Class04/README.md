# JavaScript Function Fundamentals

This repository covers essential concepts related to functions in JavaScript, showcasing key features and best practices.

## Table of Contents

1. [Function Overloading in JavaScript](#function-overloading)
2. [Rest and Spread Operators](#rest-and-spread-operators)
3. [Functions as First-Class Citizens](#functions-as-first-class-citizens)
4. [Types of Functions](#types-of-functions)
5. [Function Statement](#function-statement)
6. [Anonymous Functions](#anonymous-functions)
7. [Named Function Expression (NFE)](#named-function-expression-nfe)
8. [Object Shorthand Syntax](#object-shorthand-syntax)
9. [Array Destructuring](#array-destructuring)
10. [Arrow Functions](#arrow-functions)

---

## 1. Function Overloading in JavaScript

Function overloading refers to the ability to define multiple functions with the same name but with different parameters or a different number of parameters. Unlike some other programming languages, JavaScript does not directly support function overloading.
JavaScript uses the rest operator, enabling a function to accept an arbitrary number of arguments of any data type.

---

## 2. Rest and Spread Operators

The rest and spread operators in JavaScript provide concise ways to work with function arguments and arrays. 
The rest operator allows a function to accept an indefinite number of arguments, while the spread operator can be used to expand elements of an array or object.

Example:

```javascript
function sum(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}

const numbers = [1, 2, 3, 4, 5];
const result = sum(...numbers);
console.log(result); // Outputs: 15
```

---

## 3. Functions as First-Class Citizens

In JavaScript, functions are first-class citizens, meaning they can be treated like any other variable. They can be assigned to variables, passed as arguments to other functions, and returned as values from functions.

```javascript
const add = function (a, b) {
  return a + b;
};

const result = add(3, 4); // Outputs: 7
```

---

## 4. Function Statement

The function statement is a way to declare a function using the `function` keyword. It is hoisted to the top of its scope during execution.

Example:

```javascript
sayHello(); // Outputs: Hello!

function sayHello() // function statement
{
  console.log('Hello!');
}
```

---

## 5. Anonymous Functions

Anonymous functions are functions without a name. They are often used as function expressions or as arguments to higher-order functions.

Example:

```javascript
const add = function (a, b) {
  return a + b;
};
```

---

## 6. Named Function Expression (NFE)

A Named Function Expression (NFE) is a function expression that includes a name, allowing the function to refer to itself from within its body.

Example:

```javascript
const factorial = function calcFactorial(n) {
  return n <= 1 ? 1 : n * calcFactorial(n - 1);
};
```

---

## 7. Object Shorthand Syntax

Object shorthand syntax is a concise way to define object properties and methods when the property name and variable name are the same.

Example:

```javascript
const name = 'John';
const age = 30;

const person = { name, age };
console.log(person); // Outputs: { name: 'John', age: 30 }
```

---

## 8. Array Destructuring

Array destructuring allows you to extract elements from arrays and assign them to variables in a single statement.

Example:

```javascript
const numbers = [1, 2, 3];
const [a, b, c] = numbers;
console.log(a, b, c); // Outputs: 1 2 3
```

---

## 9. Arrow Functions

Arrow functions provide a concise syntax for writing functions, with implicit returns and a lexically scoped `this` keyword.

Example:

```javascript
const add = (a, b) => a + b;
console.log(add(3, 4)); // Outputs: 7
```
