# Compass Notes
*Dec 1st, 2021*
## Jest functions
  * if we want to group a series of tests, wrap them all in a `describe()` function
  * `it()` function is an alias to the `test()` function, therefor they are interchangeable
  * `xit()` and `test.skip()` are used to replace `it()` and `test()` when skipping tests
## Jest commands
Available watch options. When we press the `w` key in watch mode, we are presented with a list of options
  * Press `a` to run all tests.
  * Press `f` to run only failed tests.
  * Press `q` to quit watch mode.
  * Press `p` to filter by a filename regex pattern. - *Runs tests in single file*
  * Press `t` to filter by a test name regex pattern. - *Runs single test*
  * Press `Enter` to trigger a test run.
## Mocking
  * Feature called mock functions, also known as "spies", replace real functions for testing
  * part of the Jest framework
  * create a basic mock in any test by calling the `jest.fn()` function
example
The function, in reality, may sum two numbers. The mock function will return 42 no matter what.
```js
it("uses the mock implementation", () => {
 const fn = jest.fn((a, b) => 42);
 fn(1, 2);
 expect(fn).toHaveReturnedWith(42);
});
```
  * We can capture the different calls made to the function and the arguments for each call.
  * We can configure the function to return any value that we want for the specific test.