# Zoom Notes
*September 21st, 2021* 
### Responsive Design
  * renders page differently according to device, eg. laptop, desktop, ipad, phone
  * viewport = visible part of the document
### SASS
  * preprocessor and complies into css file for browser support
  * all the functionality of css with additional options
  * scripting language that extends css allowing developers to write code in one language then compile into css
  * `.scss` extension
  * sass is not native css, therefor, it needs to be installed
  * sass in run in terminal with input output for creating css files. `sass input.scss output.css` eg. `sass nav.scss nav.css`
  * sass option *watchmode* allows for automatic conversion
  * sass has variable available for use in css. sass variable syntax `$variable-name: value;`, e.g `$primary-color: aquamarine;`
  * sass allows for nesting of css selectors
  * nesting exmaples
```scss
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```
```css
nav ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
nav li {
  display: inline-block;
}
nav a {
  display: block;
  padding: 6px 12px;
  text-decoration: none;
}
```