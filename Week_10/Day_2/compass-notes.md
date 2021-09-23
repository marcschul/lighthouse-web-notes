# Compass notes
*September 21st, 2021*
### Algorithms
  * set of instructions or steps for accomplishing a specific task.
  * is any piece of code that performs a particular task or solves a particular problem
  * e.g `console.log("Hello World");` is an algorithm

### Algorithm Complexity
  * How fast or slow a particular algorithm is measured in number of elementary operations.

### Elementary Operations

  * simple operations that take a fixed amount of time to perform

```js
let result = 0; // 1
result += number1; // 1
result += number2; // 1
console.log(result); // 1
// Total of 4 elementary operations
// Running time of 4
```

### Running time
  * count of all of the elementary operations that an algorithm performs
  * if a an algorithm performs `n` elementary operations, we say the running time is `n`.
  * **time complexity** is often referred to as running time


### `n`
  * `n` === data's input size
  * Array's have `n` elementary operations, where `n === array.length`

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

// n + 1, the +1 is an extra check at the end in order to stop the loop
// 3 + (n * 3) + n + 1
// Can be simplified with math
// Running time of 4n + 4
```

### `O()` - Big O Notation
  * Algorithmic efficiency
  * How fast a function grows or declines
  * Only care about arbitrarily large input
  * Drop the Non-Dominant Terms
  * Drop Constants eg. `1`

|`O` running times| Complexity | Rate of Growth |
|---|---|---|
|`O(1)`| constant	| none |
|`O(n)`| linear time | fast|
|`O(log n)`| logarithmic | |
|`O(2^n)`| exponential | |
|`O(n^2)`| quadratic | |
|`O(n^3)`| cubic | |
|`O(n!)`|	factorial	slow | slow |