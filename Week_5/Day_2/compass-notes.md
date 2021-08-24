# Compass notes
*August 17th, 2021*
## Networking
  * every time our browser accesses a website, it makes an HTTP request by opening a TCP connection on port 80 (or 443 for https) to a given HTTP server's IP address. It then sends text-based commands such as GET /path-to-page HTTP/1.1\r\n along with many other request headers (such as the user agent string, etc.) and waits for a response from the server.
  * `request` module simplifies the process of http requests. It's not built in, so a npm install is required.
### JSON - Javascript Object Notation
  * a subset of javascript used
  * a lightweight subset of javascript used as a **text only** data-interchange format that is completely language independent
  * Easy for machines to parse and generate
  * Language independent
  * Built on two structures
    * A collection of name/value pairs.
    * An ordered list of values.
  * in JSON, property key's are always strings wrapped in quotes
    * JSON example: `'{"name":"John", "age":30, "car":null}'`
  * `JSON.parse()` converts a string type into an object type
  * `JSON.stringify()` converts an object type into a string type
  * `JSON.parse()` and `JSON.stringify()` are inverse functions to each other
  * XML is an alternative, used in older system. JSON > XML

### SSH - Secure Socket Shell
  * SSH, also known as Secure Shell or Secure Socket Shell, is a network protocol that gives users, particularly system administrators, a secure way to access a computer over an unsecured network
  * Secure Shell provides strong password authentication and public key authentication, as well as encrypted data communications between two computers connecting over an open network, such as the internet.


