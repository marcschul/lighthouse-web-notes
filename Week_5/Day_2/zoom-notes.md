# Zoom Notes
*August 17th, 2021* 
## Networking
  * Internet - Network(Hardware) vs WWW, world wide web, webpages(software)
  * HTTP, TCP, FTP, IP, MAC Address
  * Protocols - a set of rules defining a way for two systems to communicate
  * Each protocol has it's own port
### IP - InternetProtocol
  * IP Address
    * Two versions, V4 / V6
    * v6 developed due to a lack ofip address
    * v4 = 000.000.000.000
    * v6 2001:db8::8a2e:370:7334
    * v6 uses hex, allowing more addresses
    * Each device has both v4, v6
    * v4 legacy - v6 new version
    * usually only 1 is used (usually v6)
### TCP - Transmission control Protocol
  * TCP Breaks down into packets(p), from different routes(nodes)
### HTTP - HyperText Transfer Protocol
  * HTTP is impletemented with IP + TCP
  * on top of TCP
  * commands: METHOD + ROUTE
  * Methods:
    * `get`
    * `post`
    * `put`
    * `delete`
  * Header and Body are key value pairs
### Servers
  * import server module `const net = require('net');`
  * Servers need client IP address and Port
  * `const server = net.createServer();` creates an object as a server
  * `server.listen(port, callback);` function applied to the server object created from `.createServer();` method. checks port constantly, for an event
  * Event is a action performed by the user
  * Event handles is a callback, when an event happens
  * usually, the `.on('nameOfEvent', callback)` method is used in node for handling events. eg: `server.on('connection', () => {console.log('Client connected')})`
  * `'connection'` and `'connect'` are different reserved words for net module
  * need client `port` and `ip` for connection
  * ip `localhost` for client and server on same machine
Example of a client.js file below
```js
const client = net.createConnection({
  port  : port,
  host  : 'localhost'
});
```
Example of using the `on` method appened to the `client` object. 
  * The name of event `'connect'` 
  * callback `console.log('Client connected to the server');` which is the event handler... defined as registering the event handler.
```js
client.on('connect', () => {
  console.log('Client connected to the server');
});
```
  * `client.write('sends a message back to the server')`

### DNS - Domain Name System
  * Domain Name Server
  * Maps a name to an IP address
  * exmaple: `www.google.com` -> DNS -> `ipaddress`

* networking protocols are built on TCP/IP protocols, layered
* Example, http, https, ftp, ssh, work on top of TCP/IP

Post man analogy for networking, ports
  1. mail package
  2. goes to ontario
  3. goes to city
  4. postman brings to apartment
  5. goes to apartment #