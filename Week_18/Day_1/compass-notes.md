# Compass Notes
*Nov 15th, 2021*
## General
3 different concepts here:

  * Resource: `{id: 42, type: employee, company: 5}`
  * Route: `localhost:8080/employees/42`
  * Endpoint: `GET localhost:8080/employees/42`

You can have different endpoints for the same route, such as `DELETE localhost:8080/employees/42` So endpoints are basically actions.

Also you can access the same resource by different routes such as `localhost:8080/companies/5/employees/`42` So a route is a way to locate a resource.
## side effects
In computer science, an operation, function or expression is said to have a side effect if it modifies some state variable value(s) outside its local environment, that is to say has an observable effect besides returning a value (the main effect) to the invoker of the operation.
## React Hook API - useEffect
  * react side effect occur every time it renders. When we talk about side effects, we're referring to things like API calls, updates to the DOM, and event listeners, among other things.
  * import useEffect \w `import React, { useEffect } from 'react'`
## React hook rules
  1. Don't call Hooks inside loops, conditions, or nested functions.
  2. Only call Hooks from inside React components.
  3. The effect method that we pass to useEffect must either return undefined or a function.
## Data fetching pattern in React
  1. The component has no results when React renders it the first time.
  2. The component makes an asynchronous request to the API server.
  3. The data for the component is returned in the response.
  4. The component can now be updated with the data using an action that sets the state.