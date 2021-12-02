# Zoom Notes
*Dec 2nd, 2021*
## Cypress for End-To-End Testing (E2E)
  * Cypress - Fast, easy and reliable testing for anything that runs in a browser.
  * Install with `npm install --save-dev cypress`
  * Run cypress with `npm run cypress`, find and define in `json.package` or `yarn.lock`
  * Cypress cheatsheet to help with syntax
`package.json` example:
```js
{
  "scripts": {
    "cy:run": "cypress run"
  }
}
```
  * `cypress.json` hold configuration files for cypress testing
`cypressjson` example:
```js 
{
  "baseUrl": "http://localhost:3000",
  "projectId": "ghvcei",
  "video": false
}
```