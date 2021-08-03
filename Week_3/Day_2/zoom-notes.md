# Zoom notes
*Augest 3rd, 2021*
## Automated Tests
  * Save Time, Cost, Money, Energy
  * Wide range of tests
## Test Driven Development (TDD)
### General
  * A software development practice which focuses on creating test cases before developing the actual code.
  1. Write Tests
  2. Test Fails
  3. Write Function
  4. Test Passes
  5. Refactor
  6. Clean Code
  7. Go back to Step 1, Repeat
  * Clearly defines the output, which helps a developer understand and define the algorithm.
  ### `Try` and `Catch`
  * The JavaScript statements `try` and `catch` come in pairs:
  * `try` statement lets you test a block of code for errors.

  * `catch` statement lets you handle the error.
  
  * `throw` statement lets you create custom errors.
  
  * `finally` statement lets you execute code,  after try and catch, regardless of the result.
  * Javascript creates error object when an error is encounter, otherwise, error object is 
  ``` JS
  try {
  // Block of code to try
}
catch(err) {
  // Block of code to handle errors
}
```
### Require and Export
  * In Javascript, you can link files with Require and Export
  * `module.exports = myVar;`
  * `const myVar = require(fileName);`
  * Generally, Developers place code in objects before require and export, so that a lot of data can be imported
### Assert in Node.js
  * Built library in to javascript for testing
  * Does not show if test fail
## Mocha and Chai
  * Mocha is a testing framework for javascript running on Node.js and in the browser
## [mochajs](https://mochajs.org/)
  * Mocha and Chai allows developers to combine the try and catch
  * Mocha is a module on npm
  * Mocha needs to be installed with npm
## [chaijs](https://www.chaijs.com)
  * Chai is a BDD / TDD assertion javascript library for node and the browser that can be paired with any javascript testing framework.
  * chai also needs to be installed `npm install chai --dev`
  * chai is not a built in asset
  * after installation, JSON.package should be updated with the chai dependencies


**Q**: catch statement error object ???
<br>
**A**: javascript creates error object when an error is encounter, otherwise, error object is undefined<br><br>
npm run test 