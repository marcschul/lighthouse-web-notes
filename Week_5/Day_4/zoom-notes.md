# Zoom Notes
*August 19th, 2021* 
### Promises & Callbacks
  * `try` and `catch` does not work with asynchronous code, so we need an alternative to test code
  * Callbacks become messy quickly
  * avoiding nested callbacks
  * Error handling becomes much simpler with promises
  * Promises make asynchronous code easier to unit test
  * `Promise.all` can be used to run multiple async operations in parallel and have a single callback to see all the results together
  * A `Promise` is in one of these states:
    * *pending*: initial state, neither fulfilled nor rejected.
    * *fulfilled*: meaning that the operation was completed successfully.
    * *rejected*: meaning that the operation failed.

### Generate a new promise

---
```js
return new Promise((resolve,reject) => {
  // code..
})
```

### FS Library for promises
  * packages can also use promises, but not all packages. For example, the js package promise would look like the following.
  ```js
  const fs = require('fs').promises;

  fs.readFile('./fileName.txt', 'utf8')
  .then ((data) => {
    // code..
  })
  ```
Nested callback code Example before refactored

---
 ```js
// clepto.js
gotoTheirHouse(billy, () => {
  pretendToBeFriends(billy, () => {
    stealWhenNotLooking(billy.mixtapes, (items) => {
      hideInBackpack(items, () => {
        console.log("I don't feel well. I gotta go home now Billy!");
      });
    });
  });
});
```
Refactored with Promises

---
```js
// clepto_promises.js
gotoTheirHouse(billy)
  .then(pretendToBeFriends)
  .then(stealWhenNotLooking)
  .then(hideInBackpack)
  .then(() => {
    console.log("I don't feel well. I gotta go home now Billy!");
  });
```