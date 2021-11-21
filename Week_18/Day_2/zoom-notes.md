# Zoom notes
*November 16th, 2021*
# React
## Side Effects
  * When a function that modifies the state of the computer or interacts with the outside world
  * changing the value of a variable which is defined outside the scope of it
  * writing data to files or terminal
  * sending requests over the network
  * interacting with DOM(eg.enable or disable a button)
## Hooks
  * Hooking into the React state
  * only top level, hooks should never be nested
  * never in conditions, loops, nested, ect. 
## Clean up function
  * add `return () => {}` to your code, to return the value
## Dependency array
  * `() => {}, [dependency array]`
  * used to target states
  * if you provide an empty array `[]` as a dependency array, it will only run the one time. Normally when a page loads.
## Lifting State
  * Bringing state up a level; (ie. previous component)
## Client, Server, Database
`Client           <--->       Server    <---> Database`
|Client|Server|Database|
|---|---|---|
|Using react, Listening on port: 8000:|Using node.js, listening on port:8001|Using psql: listening on port:5432|
|http requests to server||server requests sql queries database|
|server responds with content||database res with data|


# Q&A
  * in react we use `{}` often, so does that mean react uses objects constantly for values?
  * in useEffect, with the `return` statement, are they similiar to promises, or replace promises entirely as we only want our code to run when certain conditions/function are finished.
  * define paradim... ?