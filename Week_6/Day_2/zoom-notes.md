# Zoom Notes
*August 24th, 2021* 
## Web Servers

### HTTP
  * Built in package of node
  * on top of TCP
  * commands: METHOD + ROUTE
  * METHODS:
    * `GET`
      * used to request data from a specified resource
      * query string (name/value pairs) is sent in the URL of a GET request
      * can be cached
      * remain in the browser history
      * can be bookmarked
      * should never be used when dealing with sensitive data
      * have length restrictions
      * are only used to request data (not modify)
    * `POST`
      * used to send data to a server to create/update a resource.
      * data sent to the server with POST is stored in the request body of the HTTP request:
        * are never cached
        * do not remain in the browser history
        * cannot be bookmarked
        * have no restrictions on data length
    * `PUT`
    * `DELETE`
  * ROUTES:
    * specifies a specific resource

### Express
  * Not a built in package of node
  * Need to `npm install express`
  * `npm init -y`
  * `"GET /"` - is an endpoint route
  * to define how application should respond to a client request for a specific endpoint, http method and event handlers
  * Express helps us with routing, template engines and middleware
  * /urls/:id creates a variable called id and stores it in req.`req.params.id`
  * Routing refers to how an application’s endpoints (URIs)
### Template Engine
  * enables us to use static template files in your app. at runtime, at the template engine replaces variables in a template file with actual values, and transforms.
  * EJS - Embedded Javascript template engine
    * wraps code with `<% Javascript code %>`
```html
<html>
<% javascript code.. %>
</html>
```
### Middleware
  * Middleware is software that enables one or more kinds of communication or connectivity between two or more applications or application components in a distributed network
  * Needs to be required and installed
  * Adds functionality to your server
  * example `app.use(morgan('dev'))`
  * 