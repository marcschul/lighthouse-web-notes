# Zoom Notes
*August 10th, 2021* 
## Asynchronous Coding
  * Javascript has asynchronous and synchronous control flows
  * FileSystems*(FS)* `const fs = require('fs')` imports a built in javascript filesystem library
  * synchronous code runs before asynchronous....?
  * JS -> callstack -> web apis -> callback queue -> callstack

Q & A:
  * **Q:** Does JS wait for all the synchronous code to evaluate before evaluating async code?

  * **A:** All synchronous code evaluates first

  * js runs top to bot, will evaluate all sync code first, then evalaute async code, which is placed in callstack -> web apis -> callbackques

## NPM
  * `npm search "my-package-name"` will list all packages associated with name
  * packages need an unique package name
  * `npm unpublish my-pack-name` to remove your npm package