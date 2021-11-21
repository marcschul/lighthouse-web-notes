# Compass Notes
*Nov 1st, 2021*
## Template Engines
  * Pure `HTML` pages are are static
  * template engines create dynamic pages
    * eg. php, ejs, ergb, liquid
  * These engines are mostly HTML with a special tag to execute code
    * eg. EJS `<%` javascript code.. `%>`

```html
  <ul>
    <% for(let i = 1; i <= 5; i++) { %>
      <li><%= i %></li>
    <% } %>
  </ul>
```

## JSX - JavaScript XML
  * React requires **component names** start with a **capital letter**.
  * `React.createElement` - Creates html elements in react
  * `ReactDOM.render` render's a view in the DOM's node using react
  * JSX is more strict than HTML

## JSX Rules
  1. All tags must be closed, There are two ways.
    * Use two tags (an open tag and a close tag - as with `<div>...</div>` below)
    * Use one self-closing tag (as with `<Album />` below)
  2. A child tag must close before its parent.
  3. No HTML comments.
  4. All JSX expressions must result in one root level element. A function can only return one value.

eg. GOOD
```js
return (
  <div>
    <input />
  </div>
)

/* becomes */

return React.createElement("div", null, React.createElement("input", null))
```
eg. BAD
```js
return (
  <div>
  </div>
  <input />
)

/* becomes? */

return (
  React.createElement("div", null)
  React.createElement("input", null)
)
```
