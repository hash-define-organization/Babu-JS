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
When a variable or a function is accessible before it was assigned its values that is called hoisting.
everything in JavaScript gets hoisted

## Execution context
