# Compass Notes
*Dec 7th, 2021*
## React
  * Client - seperate from backend
  * many apis...
## React Router
  * handles front-end routes without reloading the page
  * www.reactrouter.com/docs
  * `import { BrowserRouter, Routes, Link } from "react-router-dom";`
  * tree structure; nested routes
eg.
```js
<BrowserRouter>
  <Routes>
    <Route path="/url" element={<Urls/>}>
    <Route path="/" element={<h2> welcome to my my homeage</h2>}>
  </Routes>
</BrowserRouter>
```
  * Path prop is path
  * element prop is component
  * Do not use href with `React` because it will reload the page by default
  * use `<Link>` instead of `href`
  * React router 5 vs 6 have difference so becareful
  * React router 6 order doesn't matter for nested routes
  * `<Link to="urls"> Urls </Link>
## React bootstrap
  * style components for you
# material ui react
  * mui.com

