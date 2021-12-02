# Zoom notes
*November 23rd, 2021*
## React Overview
  * `npx create-react-app name` creates a new react app in a directory named name
## Packages
  * `Sass` - css styling
  * `Axios` - api calls

## Weather API response
  * API's JSON object


## Data structure
```jsx
interface TodoListItem {
  id: number,
  name: string,
  description: string,
  isComplete: boolean
}

interface TodoList {
  interface TodoList {
    id: TodoListItem
  }
}
```
interface comes from typescript

## HTML Structure
  * -body
      -header
        -title
        -current weather
          -city
          -temp
          -description
      -main
        -form
          -name
          -description
          -button
        -ul
          -li
            -name
            -description
            -button marking complete
            -button delete

## Component Structure
  -App
    -Header
      -WeatherWidget
    -todoForm
    -todoList
      -todoListItem

## Steps