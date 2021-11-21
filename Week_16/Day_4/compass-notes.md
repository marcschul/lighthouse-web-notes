# Compass Notes
*November 4th , 2021*
## React
### `npx` - Node Package eXecutable
  * `npx create-react-app` runs the a npx to create a react project.
### Events
  * events in react are always camalCase eg. `onSubmit`
  * events can be anon inline functions or declared outside the html
### Data Structures
  * React uses data structures
  * ds = [Array, Tree, Object, Map]
  * Key difference between object and map. Maps are ordered and iterable, while objects are not
  * Arrays are useful when order of data is important
  * Objects are useful when description is important
### React Properties
  * Passed two ways
    * `key=value` pairs, eg `<Profile firstName="Amy" />`
    * spread operator to destructure an object `{...{key: value}}` eg. `<Profile {...user} />` 
    * Both examples have the same effect, yet the syntax is different.
  * DO NOT CALL THE FUNCTION with `()` while passing the prop to html
  * `props` object in react has built-in children key `props.children` contains **anything that is is inside the tags of a component**
  * `props.children` is anything that is passed to a component inside its tags. Within any component.
### React State
  * In computer science, the state of a program is defined as its condition regarding stored inputs.
  * To store state, we need to use a feature of React called "hooks" - specifically, the `useState` hook.
  * to use state `import React, { useState } from "react";`
  * `const [count, setCount] = useState(0);` uses array destructing on left side of the assignment operator
  * React Hook States use `getter` 'gets a value' and `setter` 'sets a value'
  * hooks are not inside conditionals, loops, or other functions, they need to be at the top of the component function.


