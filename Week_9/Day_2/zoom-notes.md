# Zoom Notes
*September 14th, 2021* 
### ajax - **A**synchronous **Ja**vascript **X**ML
  * AJAX allows web pages to be updated asynchronously by exchanging data with a web server behind the scenes. 
  * AJAX is not a programming language.
  * Read data from a web server - after the page has loaded
  * Update a web page without reloading the page
  * Send data to a web server - in the background
  * AJax uses `XMLHttpRequest (XHR)` objects
  
### JQuery Ajax
```js
$.ajax({
  url: url, // "/tweet", ....
  method: method, // "GET", "POST", ect...
  data: data, // data
  success: success, // success
  dataType: dataType // "json", "xhml"
});
```
// .catch?