# Objects in JavaScript
An object is a complex data type that allows you to store and organize data using key-value pairs. Objects in JavaScript are instances of the `Object` class and can represent real-world entities in a program. Objects are a fundamental part of the language and play a central role in JavaScript programming.

An Object can be created using an object literal `{}`

for example:
```js
const person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30,
  sayHello: function() {
    console.log('Hello!');
  }
};
```
## Autoboxing
Autoboxing happens when you attempt to access a property or method on a primitive value. JavaScript creates an object wrapper around the primitive value, allowing you to use properties and methods normally associated with objects.

```js
// Autoboxing in JavaScript
let primitiveString = "Hello";
let stringObject = new String(primitiveString);  // Explicitly creating a String object

let length = primitiveString.length;  // Autoboxing (implicit conversion)

console.log(length);  // Output: 5
```

It's important to note that autoboxing in JavaScript is generally a transparent process to the developer, occurring implicitly when needed. However, explicit conversion to objects is also possible, as shown in the second example.

## Hoisting
When a variable or a function is accessible before it was assigned its values is called hoisting.
everything in JavaScript gets hoisted

## Execution context
JavaScript engine creates a special environment to handle the parsing and execution of this JavaScript code. This environment is known as the Execution Context.

## Global Execution Context
The global execution context is top-level execution context in a programming environment. 
It represents global scope of a program, meaning that variables declared here are accessible throughout the entire codebase. 
The global execution context is created when a program starts running and remains active until the program terminates.

## Lexical Scope
It is the scope of function's scope + parent's scope.
Variable's Reference is passed in lexical scope.

## Variable Declaration
Originally, the only way to declare variables was by using 'var'.
In ES6, let & const were added.

## Temporal Dead Zone (TDZ)
let and const are hoisted in JavaScript but are stored in the Temporal Dead Zone (TDZ) until execution reaches the line where the variables are initialized,
making them inaccessible before that point.

```js
  // Example with 'let'
  console.log(x); // ReferenceError: Cannot access 'x' before initialization
  let x = 5;      // Variable 'x' is hoisted to the TDZ until this line is reached
  console.log(x); // Outputs: 5

  // Example with 'const'
  // console.log(y); // ReferenceError: Cannot access 'y' before initialization
  const y = 10;    // Variable 'y' is hoisted to the TDZ until this line is reached
  console.log(y);   // Outputs: 10
```

## Autoglobal
When a variable is initialized without var, let or const, it automatically becomes a global variable.

```js
function exampleFunction() {
  // No keyword (var, let, const) used, so 'implicitGlobal' becomes a global variable.
  implicitGlobal = 'I am global';
}

exampleFunction(); // The variable 'implicitGlobal' is now accessible globally.
console.log(implicitGlobal); // Outputs: 'I am global'
```
