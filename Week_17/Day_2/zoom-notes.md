# Zoom notes
*November 9th, 2021*
## Component based UI with React
### ES6 Features

### Property Shorthand
  * Property Shorthand
eg.
```js
let cat = 'meow';
let dog = 'woof';

let obj {
  cat,
  dog
};
// obj.cat => 'meow';
```

### Spread Operator
  * Spread operator `...`
  * used when not passing the whole obj/array
  * used on iterable data
  * use spread to access all properties or elements
  * obj = `{...objName}` passes all properties
  * array = `[...arrName]` passes all elements
eg.
```js
function sum(x, y, z) {
  return x + y + z;
}

const numbers = [1, 2, 3];

sum(numbers[0], numbers[1], numbers[2]);
sum(...numbers); // => 6
```
### Array/Object destructing
  * Array/object destructing
  * unpacks iterable data
```js
// exmaples of destructing an object and array;
import { somethingToUnpack } from "react"
const [value, setValue] = useState('');
```

### React

  * Components; Are usually nested with the convention `list`, eg. plant and plantList
  * React will not accept components starting in lowercase
  * `.js` && `.jsx` will both compile the same
  * `.jsx` will help code jsx files in various ways like auto-completing html tags
  * `.jsx` will help identify a file is written in jsx
  * wrapping code in `<></>` is considered a fragment.
  * fragments are used because react requires a single parent is returned
  * `.map` and `Object.values` `.filter` methods are helpful for React while building out multiple components

### Controlled components
  * uses it's state as only source of truth
  * `import { useState } from "react";`
  * `const [value, setValue] = useState('');`
  * shows the state, and update the state

### Storybook
  * platform that allows developers to create components in isolation
  * developers can test components in storybook
```js
// creates module
storiesOf("testName", module)

// adds a test to storybook
.add("description of test", () => { callback to test });



### Chrome install app
install react dev tools chrome