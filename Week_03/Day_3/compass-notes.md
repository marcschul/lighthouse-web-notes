# Compass Notes
*August 4th, 2021*
## TDD
  * Modules vs Libraries vs Packages
    * Library is a collection of code stored in a single file (can also be called packaged library)
    * Packages is a library, that can be stored in a single file or multiple files
    * Modules logically group functions into separate files. reduce duplicated code and encourage modularity


  * Javascript's `require` method
## Mocha and Chai
  * Mocha's `describe` Function
  * Mocha's `it` Function
  * Chai's `assert` ... ?
  ``` JS
  const chai = require('chai');
  const assert = chai.assert;
  ```
  * exports fn
  ``` JS
  module.exports = myFuncName
  ```
  * importing library to a JS File
  ```JS
  const library = require('library');
  ```
  * Javascript `module` object

## Object Oriented Programming (OOP) 

  * JavaScript has multiple paradigms; initially popularized Functional Programming but was also object-oriented.
  OO is a software development paradigm
  * OO is a popular way to solve code organization, re-use and modularity
  * OO is very important to learn due to its popularity
  * JavaScript is not strictly OO in the way that Java or Ruby are
  * Functional Programming is an alternative paradigm, and one that JavaScript also encourages
  * OO bundles together state and logic into an object that can be represented as a single variable
### State *(properties)* & Behaviors *(methods)*
---
  * **State** tells us how the object looks orwhat properties it has.
  * **State** takes the form of information(Data)
  * **Behavior** tells us what the object does.
  * **Behavior** takes the form of methods(Data structures)

## Classes

  * class syntax es6, in es5 and before, prototypes were used
  * to create a new object from a class, we use the `new` keyword:
  * The difference between classes and instances
    * classes are templates of objects
    * instances are the object itself
### Creates a object from a class
---
``` JS
let pizza1 = new Pizza();
let pizza2 = new Pizza();
```
### Adds a method to a class
---
  ``` JS
  class SomeClass {
    methodName(parameters) {
      // this is method
    }
  }
```
### Adds properties to a class
---
``` Javascript
class SomeClass {
  someMethod() {
    this.hello = "hi"; // property called hello
  }
}
```
### Constructor Method
  * constructor is a special kind of method that gets executed when an object instance is created from a class.
  * constructor is for setting default values for any new object's properties.

``` js
class Pizza {
  // constructor with params
  constructor(size, crust) {
    this.size = size;
    this.crust = crust;
    this.toppings = ["cheese"];
  }
  // creates a method
  addTopping(topping) {
    this.toppings.push(topping);
  }

}
// create instance using args
let pizza = new Pizza('large', 'thin');
```
### Instance *(object)* is generated from above code
---
``` js
let pizza = {
  size: 'large',
  crust: 'thin',
  toppings: ["cheese"]
}
```
