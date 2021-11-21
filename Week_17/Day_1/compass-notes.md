# Compass Notes
*Nov 8th, 2021*
## React Tooling
  * Babel: The JavaScript Compiler
  * Webpack: The Module Bundler
  *  `npx create-react-app`, don't require us to learn how to configure a project. However, behind the scenes webpack and babel are providing the compiling and bundling capabilities needed for the project.
  * tools like these to alter source code before deployment
    * Embed environment variables into the code at build time
    * Remove code that does not ever get run
    * Use features of JavaScript that aren't standard
## Storybook
  * tool that is designed to reduce complexity in large scale applications.
  * provides a visual test environment for us to build our components in isolation
  * Framework Agnostic, ie. works with Vue, Angular, Ember, React, ect.
### JSX
  *  JSX considers that writing the name of the prop is sufficient to be considered truthy
  * eg. is sufficient 
  ```js
  <Button danger>Cancel</Button>
  ```
  * 