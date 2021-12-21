# Zoom Notes
*August 26th, 2021* 
## Web Servers
#### Routes

A route is made up of a `VERB` and a `PATH`.

Verbs: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`

- for PUT, PATCH you'll need method over-ride

[Method-override](https://www.npmjs.com/package/method-override) - can over write, `req-method`, can add `UPDATE`, and `DELETE` requests to be handled.

However we will be using only `GET` and `POST` to achive the same   

#### REST

`REST` means that the path that we are going to should represent the data being transferred. An API that uses the `REST` convention is said to be RESTful.

"RESTful routes provides a design pattern that allows for easy data manipulation. It's nicer for users and nicer for developers to have everything consistent. A RESTful route is a route that provides mapping between HTTP verbs (get, post, put, delete, patch) to controller CRUD actions (create, read, update, delete)." - [Google Search for Why Restful Routing](https://learn.co/lessons/sinatra-restful-routes-readme#:~:text=RESTful%20routes%20provides%20a%20design,read%2C%20update%2C%20delete).)

### EJS
- Embeded Javascript
- <% %>: for logic, non-outputting
- <%= %>: will output some javascript
- Template variables allow you to send data from the serve and only display it conditionally in the client
```html
<!-- logic, non-outputting -->
<% my_secret = 1234%>
<!-- output -->
<%= my_secret %>
<!-- 
expected output in browser // => 1234 
-->
```
## 
- a tag - can only do a get request
req.body.myName === name="myName"