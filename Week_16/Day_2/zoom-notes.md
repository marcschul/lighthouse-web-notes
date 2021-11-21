# Zoom Notes
*Nov 2nd, 2021* 
## React Introduction
  * A popular javascript library for ui
  * React native is using react to create mobile applications
  * Declarative programming ( as apposed to imperative programming)
  * Component base - Build once and reuse!

## Building React Projects
  * Installing React `npx create-react-app my-first-app`
  * `npx` node package runner tool, npx less overhead vs npm
    * eg, `npm start` runs all your packages with npx

## Javascript XML - JSX
  * `XML` - extensible markup language
    * XML Can be declare new elements, eg. `<flower></flower>`
  * `JSX` allows us to create dynamic pages compared to pure static html pages
  * es6 - pair of curly brackets for javascript code `{}`
  * `<React.StrictMode>` Provides better errors
  * `document.getElementById('root')` Gets the DOM element
  * `class` is a reservered word in JS, so we use `className` in React
  * Event handlers are all camalCase in React `onClick`, unlike JQuery

## Javascript
  * Closure - Changing a variable outside of scope with a function
  * State in react simply means data; 
  * `import { useState } from 'react';` imports states function from react
  * `const [keepData, ChangeData] = useState(arg)` uses the state function
  * setters and getters are part of programming, using set is a convention for React
  * component's use the convetion `props` when delcaring functions
  eg. `const myFnc = (props) => {return(<element></element>)}`

## Questions
  * Stretch: Go to react homepage and go through tutorial

  * Question: ? `${}` syntax is a template literal and place holders for es6, which will evaluate the javascript and show a result. compared to using {} which will insert javascript code for the behavior of javascript. --- is that fair?

  * Q: no yarn.lock ?

  * Q: lecture on thursday?

