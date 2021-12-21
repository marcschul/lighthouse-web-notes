## Functions
Functions, like everything else, is a value in JS. As a result, They can be store in a variable
  * Function Declaration
      * declare a func with it's keyword `function`
  * Function Expression
      * stores a func in a variable
  * Anonymous Function
      * Function not bound to an identifier, often inline or callback
      * limited and can't be used in all situations.
  * Inline Function
      * assigned to a variable and so it can be reused
  * Arrow Function Expressions
      * ES6 syntax, Special cases with `this` keyword
  * implicit return
      * returned values without using the `return` keyword
  * Callbacks
      * a function parsed in as an argument in another function
  * Higher order functions
    * takes in another function as an argument
```js
// function declaration
function myFunc1(a, b) {
  a = 'Hello '
  b = 'myFunc1'
  console.log(a + b);
};
myFunc1(); // => Hello myFunc1

// function expression
const myFunc2 = function(a, b) {
  a = 'Hello '
  b = 'myFunc2'
  console.log(a + b);
};
myFunc2(); // => Hello myFunc2

// function constructor
const myFunc3 = new Function(
  'a', 'b', 'console.log(a + b)'
);
myFunc3('Hello ', 'myFunc3'); // => Hello myFunc3

// arrow function
myFunc4 = (a, b) => {
  a = 'Hello '
  b = 'myFunc4'
  console.log(a + b);
};
myFunc4(); // => Hello myFunc4
```