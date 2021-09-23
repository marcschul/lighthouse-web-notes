# Compass notes
*September 20th, 2021*
### Algorithms
  * set of instructions or steps for accomplishing a specific task.
  * is any piece of code that performs a particular task or solves a particular problem
  * e.g `console.log("Hello World");` is an algorithm
### Algorithm Complexity
  * measure of how long an algorithm would take to complete given an input of size n
### Elementary Operations
  * any operation that takes a fixed amount of time to perform, no matter what the data is
  * Time complexity is commonly estimated by counting the number of elementary operations performed by an algorithm. It takes a fixed amount of time to perform an elementary operation.
  * Time complexity is often referred to as **running time**
  * count up all of the elementary operations that an algorithm performs and call that its **running time**
  * Algorithms that iterate over data, involve using `n` based on the size of the data
```js
let result = 0; // 1
result += number1; // 1
result += number2; // 1
console.log(result); // 1
//Running time of 4
```
```js
let result = 0; // 1

for (
  let i = 0; // 1
  i < array.length; // n + 1
  i++ // n
) {
  let number = array[i]; // n
  result += number; // n
}

console.log(result); // 1
// 3 + (n * 3) + n + 1
// Can be simplified with math
// Running time of 4n + 4
```

