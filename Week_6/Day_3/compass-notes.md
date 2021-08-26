# Compass notes
*August 24th, 2021*
## General
### Nodemon
  * utility that will monitor for any changes in our source code and automatically restart our server.
  * `npm install --save-dev nodemon`
    * installs as a developer dependency
  * `./node_modules/.bin/nodemon -L express_server.js` starts nodemon
    * the `-L` flag is used for files in a shared filesystem such as vagrant
  
### Web Servers
  * req.body takes from body
  * req.params takes from address bar
  // git reset head