# Heroku

1. add port to your express server file
```js
const PORT = process.env.PORT || 8080;
```

2. Ensure `npm start` is enable to correct path in your json.package
```json
  "scripts": {
    "start": "node filepath.js",
```