# Compass notes
*August 9th, 2021*
## [Object Orientated Programming](https://en.wikipedia.org/wiki/Object-oriented_programming)
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. ... The organization of an object-oriented program also makes the method beneficial to collaborative development, where projects are divided into groups.
### Method Overriding and Super
  * When a subclass implements a method that already exists in the superclass, it is called **method overriding** 
  * `super` keyword allows you to access the superclass
  * `super` can be used in overriding methods in order to avoid repeating code that's already present in the superclass.
### `get` and `set` Keywords
  * The `get` and `set` keywords just make our object's interface more simple.
  * `set` keyword allows Setters to validate data before assigning it to a property
  * `get` keyword allows us to compute a value on the fly instead of simply pulling it out of a property.

## Dependency Injection
  * object receives other objects that it depends on, called dependencies. The 'injection' refers to the passing of a dependency (a service) into the client that uses it.

## Abstraction
  * technique for arranging complexity of computer systems. It works by establishing a level of complexity on which a person interacts with the system, suppressing the more complex details below the current level.
  * If we add an `_` to the start of a property name, other developers will know that they shouldn't access it directly

## Single Responsibility Principle
  * a class should be responsible for a single part of the app's functionality

## Inheritance
  * Use inheritance to reduce duplicate code and share behaviour between classes

## Mocha and Chai
  * Mocha gives us the `describe` and `it` functions. Each it is a test, and each test should have at least one assertion.
  * Chai is an assertion library. It gives us assertion functions so that we no longer have to use our assertEqual and other assertion functions that we implemented previously. Chai assertion functions are deliberately designed to play nice with testing frameworks like Mocha.

## Q&A
  * Does eqArrays need to import assertEquals... ? Only the test file needs it. We recreate assertArraysEquals..
  
