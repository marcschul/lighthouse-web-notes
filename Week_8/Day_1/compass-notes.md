# Compass notes
*September 3rd, 2021*
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
  * 
