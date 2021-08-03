# Compass Notes
*August 2nd, 2021*
## Pair Programming
  * VSCode LiveShare
  * SoftSkills
    * Know your audience
      * Ask preferred pronoun
      * Little small talk, or a lot?
      * Use your judgement
    * IceBreakers
        * Ask about family
        * Ask Hobby
        * Introduce yourself
        * Don't talk about politics or Religion
    * 3 Gates of Information before talking
        1. Is it necessary to say?
        3. Is it true?
        3. Can you say it with kindness?
## Compass
### `this` Keyword
  * `this` keyword refers to the object the method (function) was called on.
  * es6 arrow function treats `this` differently
  * A common pattern in programming is to group related data and functions together under a single object in Object Oriented Programming
  ``` javascript
  const test = {
  prop: 42,
  func: function() {
    return this.prop;
  },
};

console.log(test.func());
// expected output: 42
```
### Recursion
* Recursion is a tool you can use as an alternative to traditional iteration using for and while loops.
* Every recursive function must have a base case and a recursive case.
Each recursive call should break down the current problem into a smaller, simpler one.
* The recursive calls must eventually reach the smallest version of the problem, the base case.
* The base case is when the problem can be solved without further recursion.
* The **recursive case** is when the function will continue to call itself. Every time the function calls itself, the input gets closer and closer to the **base case**. 
```javascript
// while Loop
let number = 0;
while (number <= 12) {
  console.log(number);
  number += 2;
}
```
```javascript
// Recursion
function countEvenToTwelve(number) {
  if (number <= 12) { // Recursive Case
    console.log(number);
    // The function will call itself again and get closer to the base case
    countEvenToTwelve(number+2);
  }
  // Base case, do nothing when number > 12
};
countEvenToTwelve(0);
```