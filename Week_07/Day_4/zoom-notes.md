# Zoom Notes
*September 2nd, 2021* 
## Security and Real World HTTP Servers

* security
* REST
* middleware
* build JSON API
* alternative to express
* review

### Security Issues
Authentication
---
// login route - POST
- create a cookie //
- system can remember // server is stateless
- Check userEmail exists
- Check password matches
- Set a cookie

### Object Destructing
```js
//object destructuring
const {email, id} = req.body
// Long form, but same code..
const email = req.body.email
const id = req.body.id
```

### Javascript Object Shorthand ES6
```js
let cat = 'Miaow';
let dog = 'Woof';
let bird = 'Peet peet';

let someObject = {
  cat,
  dog,
  bird
}

console.log(someObject);
//{
//  cat: "Miaow",
//  dog: "Woof",
//  bird: "Peet peet"
//}
```