# Compass Notes
*Dec 16th, 2021*
## OOP - Object Oriented Programming
  * organizes software design around data, or objects, rather than functions and logic.
  * An object can be defined as a data field that has unique attributes and behavior.
  * 
## Encapsulation
  * hiding pieces of functionality and making it unavailable to the rest of the code base.
  * form of data protection
  * creating objects and exposing interfaces (i.e., methods) to interact with those objects
## Polymorphism
  * ability for different types of data to respond to a common interface
  * "Poly" stands for "many" and "morph" stands for "forms". OOP gives us flexibility in using pre-written code for new purposes.
## inheritance 
  * class inherits the behaviors of another class, referred to as the **superclass**
## Ruby - Not EVERYTHING is an object
  * methods, blocks, and variables are not objects for example
## Ruby Classes
```ruby
# creates a new class
class GoodDog
end

# creates a variable labelled sparky, with an instance of the GoodDog class
sparky = GoodDog.new
```
## instantiation
  * creating an instance from a class
  * we've instantiated an object called `sparky` from the class `GoodDog` with the method `.new`
## Modules
  * a collection of behaviors that is usable in other classes via `mixins`
  * module is "mixed in" to a class using the `include` method invocation
## Method Lookup
  * We can use the `ancestors` method on any class to find out the method lookup chain.
    * eg. `className.ancestors`, `GoodDog.ancestors`
  
