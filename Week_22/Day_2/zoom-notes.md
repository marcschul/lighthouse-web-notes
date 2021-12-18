# Compass Notes
*Dec 14th, 2021*
## Ruby Intro
### MVC - Model View Controller
a software design pattern commonly used for developing user interfaces that divide the related program logic into three interconnected elements. 
  1. The Model
  2. The View
  3. The Controller

  * run ruby in vagrant
  * `ruby -v` ruby's version
  * `rvm` ruby version manager
  * `irb` ruby's shell

### Variables
```ruby
name = "Marc"
puts name

Name = "John"
puts Name
```
* `"hello".class` will output string.

* Data types in ruby are not coerced like javascript
* Everything in Ruby is an Object
* snake_case is the convention in Ruby
* concatenation in ruby uses the `+` operator
  * eg. `puts name + " " + name` or `puts "#{name} #{last_name}"`
* single quotation is not acceptable for concats
* `#` syntax for commenting
* 

### Conditionals
```ruby
num = 7

if(num > 6)
  puts "it's smaller than 6"
end

if num > 6  || num < 0 

    puts "In a good range!"

elsif num < 5
    puts "still not bad"

else
    puts "please change it"

end

username = "Matt"
unless username == "Anh"
  puts "choose a better username"
end

raining = true
puts raining ? "It's raining" : "It's sunny!"

```

  * Parentheses are optionally
  * `unless` the opposite of if
  * Ruby uses `elsif` with no e

### Loops
```ruby
counter = 0

loop do
    puts "The counter is #{counter}"
    counter += 1
end

while counter < 10
    puts "The counter is #{counter}"
    counter += 1
end

until counter > 10
    puts "The counter is #{counter}"
    counter += 1
end


dogs = ["Bita", "Milo", "Cocoa"]
dogs.each do |dog|
    puts dog
end


(1...10).each do |num|
    puts num
end

```
  * `loop do` syntax for loop iteration
  * `until` syntax, until condition is true
  * `while` syntax, while condition is false
  * `do` defining arguments for a block

### Methods
```ruby
def say_hello(name, last_name)
    puts "Hello #{name} #{last_name}"
end

say_hello("Warren", "Uhrich")


def double(num)
    num = num * num
    puts num
    return num
end

myNum = 10
puts double myNum
puts myNum
get_the_date birth_date, place, 


```

  * `variable_name.methods` shows available methods
  * `say_hello` and `say_hello()` are the same. ie. parenthesis are optional
  * without parenthesis without `()` may make it difficult to id the function
  * last line of your function will return a value
  * `p` and `puts` are slightly different both print

### Hashes
  * A collection of key value pairs
  * Object: the instance of a class which can have properties and methods
```ruby
hash_name = {
  "key_name" => "value",
  "key2_name" => "value2"
}

my_key_variable = 'value_key'
puts hash_name['key_name']
puts hash_name[my_key_variable]


betteruser = {
    :username => 'Mahsa',
    :password => '1235'
}

puts betteruser[:username]

modern_user = {
    username: "Mahsa",
    password: '54321'
}

puts modern_use
```

### Blocks and Lambdas
```ruby
dogs = ["Bita", "Milo", "Cocoa"]


greeting = lambda do |name|
puts "Hello #{name}" 
end

greeting.call "Brett"
```

  * Lambdas are anon functions in ruby
  * Lambdas allow you to do a quick throw function
  * Lambdas provide a way to write closures.
  * 

### Classes
```ruby
class Shape 
    def initialize initial_color
        @color = initial_color
    end

    # Getter
    def color
        @color
    end

    # Getter, different syntax, same result
    attr_reader :color

    # Setter
    def color= new_color
        @color = new_color
    end

    # Setter, different syntaxe, same result
    attr_writer :color

    # setter && getter
    attr_accessor :color
end

myShape = Shape.new 'pink'
p myShape
p myShape.color
myShape.color = 'green'
```
  * ruby uses initialize instead of `constructor()` found in js
  * `.new` method is used to generate a new class in ruby
  * `@` syntax; The variable which name begins which the character `@', is an instance variable of self. Instance variables are belong to the certain object. Non-initialized instance variables has value nil.

### Q&A

  * What exactly is `do`?
  * can we manually assign memory in ruby?
