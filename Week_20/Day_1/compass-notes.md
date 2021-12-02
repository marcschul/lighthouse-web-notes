# Compass Notes
*Nov 29th, 2021*
## Testing
  * improves work flows in large applications
  * write tests, not too many, mostly integration
  * write enough test for confidence
  * software will determine how much testing is required.
## Automated testing
  * testing will be specific to the software
  * automating testing is a way to DRY up your testing procedures
  * does not replace manual testing, rather adds to testing suite
  * common when applications grow in complexity
## regression testing
  * a process of verifying that previously uncovered bugs have not returned in new versions of software
## Types of tests
|#|Test|Speed|Cost|
|---|---|---|---|
|1|Static|Fast|Cheap|
|2|Unit|||
|3|Integration|||
|4|End-To-End|Slow|Expensive|
## Static Testing
  * Static analysis tools, eg. ESLint, Prettier
  * superset of Javascript, eg. TypeScript, Flow introduce static type checking
  * immediate feedback identifies common syntax errors
## Unit Testing
  * goal is to test a specific function or component in isolation
  * eg. using storybook to write tests for components
## Integration Testing
  * process of proving that two or more units of code work together
  * test the logic at the intersection of multiple components
## End-To-End Testing
  * as close to simulated user behavior as possible
  * higher cost of implementation, maintenance, and runtime
  * replace the manual process used to test common user flows
## TDD Test Driven Development
  * Write new code only if an automated test has failed
  * Eliminate duplication
  * Process of TDD
  1. Red - Write a small test that doesn't pass. (write test first)
  2. Green - Do the minimal amount of work to make the test pass. (make test pass)
  3. Refactor - Improve the code, continuing to ensure all tests still pass. (refactor code)
## React prop-types
  * library used in place of typescript and flow for React
  * checks props for their data structures / datatypes
## Jest
  * Testing with jest is often completed with many different libraries and functions
  * Uses a combination of queries and matchers
  * Jest `Queries` are the methods that Testing Library gives you to find elements on the page
  * Jest `Matchers` are methods that let you test values in different ways.
## Continuous Integration
  * tests run automatically after each commit 
