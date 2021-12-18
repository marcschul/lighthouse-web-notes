# Compass Notes
*Dec 16th, 2021*
## Ruby Blocks
  * arguments are how we pass in data to methods, blocks are how we pass in behavior.
  * chunk of logic that your method can run.
  * blocks are similar to callbacks in javascript, ie. passing in a function as an function argument
## Constants && Name Spacing
  * Constants refers to something different in Ruby than it does in most other languages, including JavaScript
  * A constant can refer to a Module, a Class or simple data like Floats and Strings
  * Capitalized words can be used to define a constant
  * NameSpacing is used heavily to limit the exposure of constants defined in the global namespace
  * The `::` Syntax is used to access constants (Modules, Classes, etc)
  * convention to only capitalize the first letter when defining Class and Module constants like `Apple`
  * convention to capitalize and underscore the entire name when defining value constants like `FOUNDED_BY`
```ruby
Math.class # => Module
Math::PI.class # => Float
Apple # => NameError: uninitialized constant Apple
```

## NameSpacing
  * set of signs (names) that are used to identify and refer to objects of various kinds
  * file system uses name spacing
    * eg. `marc/projects` and `marc/notes`
  * Instead of having a global names/variables, subsets are created
  *  unlike in some other languages like JavaScript, there is no variable reference pointing to the contents of the library.

### Javascript
```js
const someLibrary = require('someLibrary');

// Now the things that the someLibrary module exports are only available via the someLibrary variable.
```

### Ruby
```ruby
require 'some_library'

# Ruby have the ability to and are expected to define constants in the global namespace! Yikes.
```
## Gems
  1. `gem install name`
  2. `require "name"` in either irb or file
```ruby
require "money"
Money # => does not throw NameError regarding constant Money
Money.constants
Money::Bank.class
Money::Bank.constants
```
  * the only constant that Money defines (and hopes for that best that it is not previously defined by another library or own code) is: `Money`
  *