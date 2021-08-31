# Compass notes
*August 31st, 2021*
### HTTP is stateless
  * Server does not remember the client's behavior
  * Server process every request like a new request
  * uses cookies to store memory
### Cookies
  * Small text file
    * // can you show me the text file location and show it's contents?
  * Key-Value pairs
  * kept in browser's memory

```js
const users = {
  user1: {
    user: 'name'
  }
}
const user = users[user]
// user will eval to undefined or value
if(user) {
  // code...
}
```
```js
const {email, name, id} = req.body
```