### Compass Notes

  * The [process.argv](https://nodejs.org/docs/latest/api/process.html#process_process_argv) property returns an array containing the command-line arguments passed when the Node.js process was launched
  * Functions can produce either
    * side effects
    * return values
    * or both
  * A pure function is a specific kind of value-producing function that not only has no side effects but also doesn’t rely on side effects from other code
  * **5 Rules** for Defining a Function (Best Practices)
      1. Give your functions precise verb/action based names
      2. Use camelCasedNames
      3. Properly indent the function code.
      4. Functions should focus on a single task.
      5. functions try to avoid reading outer scope variables to make them more re-usable.