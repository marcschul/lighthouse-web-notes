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
   class that is inheriting behavior is called the **subclass**
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
## Constructor
  * a special method of the class which gets automatically invoked whenever an instance of the class is created
## Instance variable
  * uses the `@` symbol to create a variable scoped to the particular instance
  * Every object's state is unique, and instance variables are how we keep track.
## Initialize method
  * The initialize method is part of the object-creation process in Ruby & it allows you to set the initial values for an object.
  * In other programming languages they call this a “constructor”. (Javascript)
## Ruby's getters and setters
  * getters and setters are a programming paradigm
  * Ruby gives us a special syntax to use it. `object_name.set_method("string")`
  * Setter methods always return the value that is passed in as an argument and ignores everything else.
  * ruby's `attr_accessor method` is a practice for refactoring getters and setters for shorter syntax.
  `attr_accessor :instance_variable_name`. one line replaced two method definitions.
  * `attr_reader` for getter methods
  * `attr_writer` for setter methods
  * All of the `attr_*` methods take a Symbol as parameters
## Ruby self
  * `self` is a special variable that points to the object that "owns" the currently executing code
  * similar to `this` in javascript
  * `self` calls a setter method to perform work within it's instance
## Class methods
  * Objects contain state, and if we have a method that does not need to deal with states, then we can just use a class method.
  * call directly on the class itself, without having to instantiate any objects
  * prepend the method name with the reserved word `self`
    * eg. `def self.what_am_i`, defines a a class method\
  * `ClassName.method_name` as an exmaple, will call a class method
## Class variables
  * class variables use `@@`, eg. `@@number = 0`
  * class level variables that pertains only to the class, and not to individual objects.
## Constants
  * constants do not change
  * define a constant by using an upper case letter at the beginning of the variable name. 
  * convention to write entire variable uppercase.
    * eg. `DOG_YEARS = 7
  * It is possible to reassign a new value to constants but Ruby will throw a warning. (unlike javascript)
## `to_s`
  * string interpolation for ruby objects
## `<` operator
  * use the `<` symbol to inherit
```ruby
# GoodDog inherit's the Animal Class
class GoodDog < Animal
end
```
## `super`
  * keyword `super` used in ruby to call superclass
##  "able"
  *  convention for Ruby is to use the "able" suffix on whatever verb describes the behavior
## Method Access Control
  * `public`, `private`, and `protected` access modifiers.
```ruby
class Animal
  def a_public_method
    "Will this work? " + self.a_protected_method
  end

  # a_protected_method now set to protected
  # private, to set method to private
  protected

  def a_protected_method
    "Yes, I'm protected!"
  end
end
```
## `Object` class
  * Every class you create inherently subclasses from class `Object`. 
  * The `Object` class is built into Ruby and comes with many critical methods.
  * Accidentally override a method that was originally defined in the Object class
  *