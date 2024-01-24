## Class 2 - Datatypes and Variables

In our second class, we delved into the fundamentals of JavaScript datatypes and variables. The session covered the following key topics:

### Primitive Datatypes

JavaScript features seven primitive datatypes, and among them are **Number**, used for both integers and floating-point numbers; String, employed for textual data; **Boolean**, representing true or false values; **Undefined**, indicating the absence of a defined value for a variable; **Null**, representing the intentional absence of any object value; **Symbol**, a unique and immutable primitive value; and **BigInt**, introduced to handle integers beyond the limit of the Number type. Each primitive type serves distinct purposes, and understanding them is fundamental to working with data in JavaScript.

JavaScript has 7 primitive datatypes:

1. **Number:**
   ```javascript
   let integerNumber = 42;
   let floatNumber = 3.14;
   ```

2. **String:**
   ```javascript
   let greeting = "Hello, ";
   let name = "Babu Js";
   let welcomeMessage = greeting + name;
   ```

3. **Boolean:**
   ```javascript
   let isTrue = true;
   let isFalse = false;
   ```

4. **Undefined:**
   ```javascript
   let uninitializedVariable;
   ```

5. **Null:**
   ```javascript
   let nullValue = null;
   ```

6. **Symbol:**
   ```javascript
   let uniqueSymbol = Symbol("uniqueSymbol");
   ```

7. **BigInt:**
   ```javascript
   let bigIntValue = 9007199254740991n;
   ```

### Non-Primitive Types

Beyond the primitive datatypes, JavaScript supports three non-primitive types: **Object, Array,** and **Function**. An **Object** is a collection of key-value pairs, allowing the organization of related data into a single entity. **Array** is a versatile ordered list that can hold elements of various types, providing dynamic and flexible data structures. **Function** represents reusable blocks of code that can be invoked with different parameters, enhancing code modularity and reusability. These non-primitive types play crucial roles in building complex and structured programs.

In addition to the primitive datatypes, we explored 3 non-primitive types:

1. **Object:**
   ```javascript
   let person = {
     firstName: "John",
     lastName: "Doe",
     age: 30,
   };
   ```

2. **Array:**
   ```javascript
   let colors = ["red", "green", "blue"];
   ```

3. **Function:**
   ```javascript
   function greet(name) {
     console.log("Hello, " + name + "!");
   }

   greet("Babu Js");
   ```

### + Operator Overloading

JavaScript exhibits **operator overloading** with the + operator. Depending on the context, it can perform addition for numerical values or concatenation for strings. Understanding this behavior is vital to avoid unexpected results and to manipulate data appropriately, especially when dealing with mixed datatypes.

```javascript
let numericAddition = 5 + 3;  // Result: 8
let stringConcatenation = "5" + "3";  // Result: "53"
```

### String Manipulation

String manipulation is a common task in programming. JavaScript offers various methods for manipulating strings, and the **substring** method is one such tool. It allows the extraction of a portion of a string based on specified indices, enabling developers to work with substrings effectively.

```javascript
let originalString = "Hello, World!";
let substring = originalString.substring(0, 5);  // Result: "Hello"
```

### NaN (Not-a-Number)

The term **NaN** stands for "Not-a-Number" and is a special value in JavaScript, usually resulting from invalid mathematical operations. It's crucial to recognize NaN and understand that it doesn't equate to itself. Handling NaN appropriately is essential in scenarios where numerical calculations may yield unexpected outcomes.

```javascript
let result = "abc" / 2;  // Result: NaN
console.log(result === result);  // Result: false (NaN is not equal to itself)
```

### Typeof Function

The **typeof** operator in JavaScript is used to determine the type of a variable. It returns a string indicating the datatype of the operand. This is useful for dynamically checking variable types, especially when dealing with user inputs or dynamic data.

```javascript
let variableType = typeof greeting;
console.log(variableType);  // Result: "string"
```

### Variable Declaration: let, const, and var

JavaScript provides three keywords for variable declaration: **let, const, and var**. 

- let declares a mutable variable, allowing its value to be changed. 
- const declares a constant variable, whose value cannot be reassigned once set.
- var is an older way to declare variables and has function-scoping behavior.

Understanding the differences between these declarations is crucial for writing robust and maintainable code.

```javascript
let mutableVariable = "I can be changed";
const constantVariable = "I can't be changed";
var legacyVariable = "I have function-scoping";

// Example of reassigning a let variable
mutableVariable = "I am changed";
```
