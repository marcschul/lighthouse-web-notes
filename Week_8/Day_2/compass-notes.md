# Compass notes
*September 7th, 2021*
## CSS Flexible Box - Flexbox
  * Flexbox (also known as CSS Flexible Box) is a layout module in CSS.
  * efficient lay out, align and distribute space among items in a container, 
  * Size ca be unknown and/or dynamic
### Display
  * browser applies default styles to our HTML elements. One of these default styles is display.
### `display:block` 
  * A block level element will take up the entire space of its parent element. It can contain other block elements or inline elements.
  * automatically creates a new line in browser
  * Example block elements
```html
paragraph <p>
headings (<h1>, <h2>, <h3>,<h4>,<h5>,<h6>)
div (<div>)
section (<section>)
footer (<footer>)
article (<article>)
paragraph (<p>)
lists (<ul>, <ol>)
nav (<nav>)
```
### `display: inline`
  * do not start a new line when they are rendered in the browser.
  * only take up as much space as the content needs
  * can't add a width, height, padding or margin to inline elements. 
  * Example inline elements
```html
span <span>
anchor (<a>)
em (<em>)
strong (<strong>)
```
### `display: inline-block`
  * doesn't automatically create a new line in the browser, but it can have a margin, padding, height, and width
### Parent Properties
  * also sometimes referred to as the container element.
  * start using Flexbox, we add the display: flex property to the parent element.
  * Can have child properties
```css
.parent {
  display: flex;
}
```