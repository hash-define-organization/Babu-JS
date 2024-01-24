# JavaScript and its history

JavaScript was created by Brendan Eich while working at Netscape Communications Corporation in 1995

## JavaScript related to Java ?
The naming of JavaScript has an interesting story. It was originally developed by Brendan Eich at Netscape in 1995 under the code name "Mocha." However, during its official release, it was renamed "LiveScript."

Around the same time, Sun Microsystems and Netscape were collaborating, and Sun wanted to capitalize on the popularity of its programming language, Java. As a result, Netscape and Sun agreed to change the name of "LiveScript" to "JavaScript" to align it with the Java language. This decision was more of a marketing strategy, and it led to some misconceptions about the relationship between JavaScript and Java.

Despite the name, JavaScript and Java are distinct programming languages with different purposes and capabilities. JavaScript's name is more of a historical artifact than an accurate reflection of its core nature and functionality.

## JavaScript works on browsers
![image](https://github.com/hash-define-organization/Babu-JS/assets/79973672/9062e2a7-2004-4db6-86db-4a6768b5b89b)

Due to multiple engines from different browsers there was a problem as they were becoming very different from each other so a governing authority was established known as ECMA.
ECMA (European Computer Manifacturing Association) sets a standard for JavaScript engines to maintain similar structure among different engines

## High Level Language
JavaScript is a highlevel language that was used for client side in starting but later was also started being used in server side too.

![image](https://github.com/hash-define-organization/Babu-JS/assets/79973672/05c529f9-e970-4e24-9cc9-55f956845604)

## Three Features of JavaScript
### Dynamic Typing:

JavaScript is a dynamically-typed language, meaning that variable types are determined at runtime. This provides flexibility in working with data since you don't need to explicitly declare the data type of a variable. For example, you can assign a string to a variable and later reassign it to a number without explicitly specifying data types.

```js
let dynamicVariable = "Hello";
console.log(dynamicVariable);  // Output: Hello

dynamicVariable = 42;
console.log(dynamicVariable);  // Output: 42
```

### Loosely Typed
JavaScript is loosely typed, allowing variables to change types during runtime. This adds to its flexibility but requires careful handling to avoid unexpected behaviors.

```js
let looselyTypedVariable = "I am a string";
console.log(looselyTypedVariable);  // Output: I am a string

looselyTypedVariable = 42;
console.log(looselyTypedVariable);  // Output: 42
```

### Compiled at Runtime
JavaScript is an interpreted language, and its code is executed by the JavaScript engine at runtime. There is no separate compilation step. This allows for flexibility but may also lead to runtime errors.

It works in two phases:-
- Compilation phase
- Execution phase

These features contribute to the flexibility and power of JavaScript in various programming scenarios.
