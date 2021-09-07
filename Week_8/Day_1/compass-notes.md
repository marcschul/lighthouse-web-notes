# Compass notes
*September 6th, 2021*
### Stack
  * collection of technologies used in a given system
  * full-stack means developers who are comfortable working with both back-end and front-end
  
Example:
|   |   |
|---|---|
| Web Server | Node.js|
| Middleware | Express |
| Template | Engine: EJS |
| Database | mongoDB |
| Hosting/Infrastructure | Heroku |

### HTML - HyperText Markup Language
  * Language that forms structure
  * Tags form elements `<tag>`
  * Elements `<tag>content</tag>`
  * Elements form a tree in the DOM
  * Each tag can have attributes `<h1 class="article">content</h1>`, In this example, the class attribute is used.
  * [html elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

### CSS - Cascading Style Sheet
  * Language that forms style
  * Provides styling, eg. size, color, font ect.
  * 3 ways to add css to a page
    * add a `style="color: red"` attribue to a tag
    * inline in head portion of html doc`<head><style>{color: red;}</style></head>`
    * link a css file with a link tag in the head. `<head><link rel="stylesheet" href="style.css"></head>`
  * elements can only have 1 unqiue ID. ID's use the hastag`#` prefix symbol. These IDs are only used 0 or 1 time in a document, for specific style. eg. `#my-id`
  * ID's are used in html elements with the `id=""` attribute
  * Elements can have many classes. Classes use the `.` dot prefix. eg. `.my-class`
  * Classes are used in html elements with the `class=""` attribute

### DOM - Document Object Model
  * DOM uses Event-Driven Architecture (EDA)
  * EDA can be EDA can be summarized as: When `X` happens, then do `Y`.
  * A working example of EDA is events and event handlers.
  * DOM is considered an object named `document`
  * `document` in google chrome dev tools console to view a website's DOM
  * `document.body` would view the body property of the object `document`
  * client side javascript enables clients to manipulate the DOM. E.G `document.body.style.backgroundColor = 'blue'` changes the background color of a webpage

### Event Propagation
Bubbling Principle
  * DOM elements are nested within other elements, in a tree-like structure, events that affects a child element bubble up through its parents.
  * When an event happens on an element, it first runs the handlers on it, then on its parent, then all the way up on other ancestors.
  * The most deeply nested element that caused the event is called a target element, accessible as event.target.
  * Not all events bubble, but most do
  * Bubbling is convenient. Don’t stop it without a real need: obvious and architecturally well thought out.
  * to stop bubbling, the method `event.stopPropagation()` is used on the event object

### JQuery - Event Handling
  * Fixes Browser Compatibility issues
  * Cleaner API
  * Events are actions such as moving their mice over the page, clicking on elements
  * Events need to be listend to
  * Listening for an event means you're waiting for the browser to tell a specific event has occurred and then you'll specify how the page should react.
  * When an event occurs, you provide a function, also known as an event handler.

**Separation of concerns:**
  * important because it keeps like pieces of code together (i.e. HTML, JS, CSS) and unlike pieces of code apart facilitating changes, enhancements, etc.

### obtrusive JavaScript
  * does not use separation of concerns: both javascript and html in same file
```html
<button onclick="alert('Hello')">Say hello</button>
```
  * listen to is specified by the button's onclick attribute, and the event handler is the alert function which alerts "Hello" to the user
Disadvantages
  * Needs constant updates and maintenance
  * not scalable

### unobtrusive JavaScript
  * uses separation of concerns: Code is in different files.

```html
<button id="helloBtn">Say hello</button>
```

```js
// Event binding using addEventListener
var helloBtn = document.getElementById( "helloBtn" );
 
helloBtn.addEventListener( "click", function( event ) {
    alert( "Hello." );
}, false );
```
  * Still have issues with version control

### JQuery 
  * abstracts away browser inconsistencies, so the above code in JQuery would be as followed;
```js
// Event binding using a convenience method
$( "#helloBtn" ).click(function( event ) {
    alert( "Hello." );
});
```
  * `$( "#helloBtn" )` code selects the button element using the `$` (a.k.a. jQuery) function returns a jQuery object.
  * The jQuery object has a bunch of methods (functions) available to it
  * one of them named `.click`, which resides in the jQuery object's prototype. 
  * We call the click method on the jQuery object and pass along an anonymous function event handler, `function( event ) {
    alert( "Hello." );
  });`that's going to be executed when a user clicks the button, alerting `"Hello."` to the user.
  * As of jQuery 1.7, all events are bound via the `on` method, whether you call it directly or whether you use an alias/shortcut method such as `bind` or `click`, which are mapped to the on method internally

### Event listening using jQuery:
```js
// The many ways to bind events with jQuery
// Attach an event handler directly to the button using jQuery's
// shorthand `click` method.
$( "#helloBtn" ).click(function( event ) {
    alert( "Hello." );
});
 
// Attach an event handler directly to the button using jQuery's
// `bind` method, passing it an event string of `click`
$( "#helloBtn" ).bind( "click", function( event ) {
    alert( "Hello." );
});
 
// As of jQuery 1.7, attach an event handler directly to the button
// using jQuery's `on` method.
$( "#helloBtn" ).on( "click", function( event ) {
    alert( "Hello." );
});
 
// As of jQuery 1.7, attach an event handler to the `body` element that
// is listening for clicks, and will respond whenever *any* button is
// clicked on the page.
$( "body" ).on({
    click: function( event ) {
        alert( "Hello." );
    }
}, "button" );
 
// An alternative to the previous example, using slightly different syntax.
$( "body" ).on( "click", "button", function( event ) {
    alert( "Hello." );
});
```