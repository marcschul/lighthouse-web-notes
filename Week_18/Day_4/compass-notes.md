# Zoom notes
*November 18th, 2021*
## Custom React Hook Rules
  * A custom Hook is a function that must start with the word "use"
  * Don't call Hooks inside loops, conditions, or nested functions
  * Only call Hooks from inside React components
## Sharing Logic Between Functions
Hooks are designed to solve an entire class of problems in React:

  * It's hard to reuse stateful logic between components.
  * Complex components grow in size.
  * Classes confuse people and machines.
  * Custom Hook can reduce the repetition in components
  * Convention to store custom Hooks in a folder called `src/hooks`
