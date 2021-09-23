# Compass notes
*September 20th, 2021*
### Responsive Design
  * Multiple approaches
  * Popular approach "Mobile First" Development, which designs an app for mobile first. It is often easier to adjust a mobile site to fit a desktop than vice-versa
  * A `“fluid”` layout is one that stretches and shrinks to fill the width of the screen.
  * A `“fixed-width”` layout is the opposite: it has the same width regardless of the screen dimensions.
### 3 Main Concerns
  * The responsive design (the mockups for each layout)
  * CSS rules for implementing each of those layouts
  * Media queries for conditionally applying those CSS rules
### Responsive web design patterns
  * web sites normally develop patterns when developing responsive web designs
  * **mostly fluid** - usually remains the same size, simply adjusting the margins on wider screens.
  * **Column drop** - full-width multi-column layouts, column drop simply stacks the columns vertically as the window width becomes too narrow for the content.
  * **Layout shifter** - responsive pattern, with multiple breakpoints across several screen widths
  * More available aswell!
### Media Queries
  * Media queries consist of a `media type` and  `media-feature`s
  * Media queries can be linked in the `.html` file or in the `css` file
  * conditionally apply styles with the CSS
  * target specific media
  * test and monitor media states
```css
/*
* example of using media queries in css
* placed at bottom of css file
*/
@media all and (max-width:600px){
  .column {
    width: 100%;
  }
  a {
    color: blue;
  }
}
```
### Em and Rem
  * alternative to using px
  * em relative to it's parent element
  * rem (root em), sized relative to font size of root element, usually the `<html>` element
### Viewport Units
  * viewport is total window area rendered by browser.
  * size and position element based on a percentage system relative the size, height and width of browser window
  * eg. `1vw` = 1% size of width of viewport
### Viewport Zooming
  * Default behavior will prevent mobile devices from using our mobile layout
  * Disable viewport zooming by adding the following element to the `<head>` your document
  ```html
  <meta name='viewport' content='width=device-width, initial-scale=1.0, maximum-scale=1.0' />
  ```
*This is a critical element that should be on every single webpage you create.*
