# Compass notes
*August 11th, 2021*
## Asynchronous Javascript
* `setTimeout((), 0)` function is an asynchronous function that allows us to run an inline or callback function with a delayed time.
```JS
setTimeout(() => {
  // print the char here
}, 1000) 
```
* The process object in Node.js is a global object that can be accessed inside any module without requiring it. 
* `stdin` = standard input
* `stdout` = standard output
* `stderr` = standard error
* `process.stdin`: a readable stream
* `process.stdout`: a writable stream
* `process.stderr`: a wriatable stream to recognize errors
```js
// prints out hello to terminal
process.stdout.write('hello\n');
```