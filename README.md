# 100 Questions about Javascript

JavaScript is one of the most popular programming languages in the world, essential for web development, and a must-know for software developers. Whether you are preparing for a job interview or brushing up on your JavaScript knowledge, this comprehensive list of 100 questions and answers will help you solidify your understanding of JavaScript.

<details>
<summary>1- What is JavaScript?</summary>

  **Answer**: JavaScript is a high-level, dynamic, untyped, and interpreted programming language. It is primarily used for creating interactive and dynamic content on web pages. JavaScript is versatile and can be used on both the client-side and server-side (Node.js).

JavaScript allows developers to create rich web applications by manipulating the DOM (Document Object Model), handling events, and communicating with servers through AJAX requests. It is also a core technology of the web, alongside HTML and CSS.

</details>


<details>
<summary>2. What are the different data types in JavaScript?</summary>

  **Answer**: 
  1. Primitive Data Types:
     - String: Represents a sequence of characters, e.g., "Hello, World!".
     - Number: Represents both integer and floating-point numbers, e.g., 42 or 3.14.
     - Boolean: Represents logical entities with two values: true or false.
     - Undefined: A variable that has been declared but not assigned a value has the type undefined.
     - Null: Represents the intentional absence of any object value, often used to indicate "no value".
     - Symbol (ES6): A unique and immutable primitive value used as the key of an object property.
     - BigInt (ES2020): Represents integers with arbitrary precision, allowing for manipulation of large integers beyond the safe integer limit for numbers.

  2. Non-Primitive Data Types:
     - Object: A collection of key-value pairs, often used to store more complex data and entities.

> Understanding these data types is crucial for variable manipulation and function execution in JavaScript.
</details>


<details>
<summary>3. What is the difference between `undefined` and `null` in JavaScript?</summary>

  **Answer**: In JavaScript, `undefined` and `null` are distinct values that represent the absence of a value, but they are used in different contexts:

`undefined`: A variable is `undefined` when it is declared but not yet assigned a value. It represents a lack of initialization.

Example:
```javascript
let a;
console.log(a); // Output: undefined
```

`null`: A variable is `null` when it is explicitly assigned a null value. It represents the intentional absence of any object or value.

Example:
```javascript
let b = null;
console.log(b); // Output: null
```

> While both `undefined` and `null` are used to denote "no value," `undefined` is usually the default state of uninitialized variables, whereas `null` is explicitly set by the programmer to indicate that a variable should have no value.
</details>

<details>
<summary> 4. What are JavaScript closures, and why are they useful? </summary>

  **Answer**: A closure is a feature in JavaScript where an inner function has access to the outer (enclosing) function's variables—even after the outer function has finished executing. Closures are created every time a function is created, at function creation time.

**How Closures Work**: Closures enable functions to "remember" their lexical scope, allowing them to access variables from their outer scope even when the function is executed outside that scope.

Example of a Closure:

```javascript
function outerFunction(outerVariable) {
  return function innerFunction(innerVariable) {
    console.log('Outer Variable: ' + outerVariable);
    console.log('Inner Variable: ' + innerVariable);
  };
}

const newFunction = outerFunction('outside');
newFunction('inside');
// Output:
// Outer Variable: outside
// Inner Variable: inside
```

In this example, `innerFunction` retains access to `outerVariable` from `outerFunction` even after `outerFunction` has finished executing.

Use Cases of Closures:
- **Data Encapsulation**: Closures can be used to create private variables or methods within a function.
- **Callbacks**: Closures are commonly used with callbacks in asynchronous programming, such as event handlers or setTimeouts.
- **Functional Programming**: Closures enable functional programming patterns, allowing functions to be composed and reused.


> Closures are powerful tools in JavaScript that enable data hiding and state management, making them essential for building complex applications.

</details>

---

## Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

### How to Contribute
* Fork the Project
* Create your Feature Branch (git checkout -b feature/AmazingFeature)
* Commit your Changes (git commit -m 'Add some AmazingFeature')
* Push to the Branch (git push origin feature/AmazingFeature)
* Open a Pull Request

### Contributor Guidelines

* Follow the coding style and guidelines laid out in the CONTRIBUTING.md file.
* Ensure that your code passes all tests before submitting.
* Keep your commits organized and clear.
* Feel free to open an issue for any feature requests or bug reports.

# Contributors
Thanks to all the amazing people who have contributed to this project!

<a href="https://github.com/holasoymalva/100-questions-about-javascript/graphs/contributors"> <img src="https://contrib.rocks/image?repo=holasoymalva/100-questions-about-javascript"/></a>

## New Contributors
We welcome new contributors to the project! If you'd like to be a part of this initiative, just follow the steps in the How to Contribute section above. We are happy to review pull requests and collaborate on improving the project together!

## License

Distributed under the MIT License. See LICENSE for more information.


