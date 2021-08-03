# Compass Notes
*August 3rd, 2021*

*Compass broken when I woke up today*
## Javascript Modules in Node
  * DRY Code - Don't Repeat Yourself
  * modules are its way of organizing code into individual files
  * every js file in node is implicitly a module
    * we can console.log(module) and see its details
  * module.exports tells node what to export from a file
      * it defaults to {}
  * we can use require with relative paths (like ./myModule)
      * it doesn't need the .js extension, as that is implied