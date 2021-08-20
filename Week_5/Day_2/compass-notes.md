# Compass notes
*August 17th, 2021*
## Networking
  * every time our browser accesses a website, it makes an HTTP request by opening a TCP connection on port 80 (or 443 for https) to a given HTTP server's IP address. It then sends text-based commands such as GET /path-to-page HTTP/1.1\r\n along with many other request headers (such as the user agent string, etc.) and waits for a response from the server.
  * `request` module simplifies the process of http requests. It's not built in, so a npm install is required.
### JSON - Javascript Object Notation
  * lightweight text data-interchange format that is completely language independent
  * Easy for machines to parse and generate
  * built on two structures
    * A collection of name/value pairs.
    * An ordered list of values.
  * language independent
  * `JSON.parse()` converts a string type into an object type
  * `JSON.stringify()` converts an object type into a string type
  * `JSON.parse()` and `JSON.stringify()` are inverse functions to each other
  * XML is an alternative, used in older system. JSON > XML
### API - Application Program Interface
  * set of requirements that govern how one application can talk to another. 
  * allows systems to work together
  * leverage the functionality of external services
  * Examples:
    * Yelp, for instance, displays nearby restaurants on a Google Map in its app
    * some video games now let players chat, post high scores and invite friends to play via Facebook, right there in the middle of a game.
    * Facebook users undoubtedly appreciate the ability to sign into many apps and Web sites using their Facebook ID—a feature that relies upon Facebook APIs to work.
  * double edge sword if your application relies on the API.
  * Rest API - Representational State Transfer
    * Call from client to server and get data back over the http protocol
  * 
### SSH - Secure Socket Shell
  * SSH, also known as Secure Shell or Secure Socket Shell, is a network protocol that gives users, particularly system administrators, a secure way to access a computer over an unsecured network
  * Secure Shell provides strong password authentication and public key authentication, as well as encrypted data communications between two computers connecting over an open network, such as the internet.


