# Compass notes
*August 23rd, 2021*
## General
### cURL - Client Uniform Resource Locator
  * cURL is a command line utility that is used to make HTTP requests to a given URL and it outputs the response
  * `curl www.example.com` will print out the html of a website
### Character Encoding
  * Character encoding provides a key to unlock (ie. crack) the code.
  * It is a set of mappings between the bytes in the computer and the characters in the character set. Without the key, the data looks like garbage.
  * **UTF-8** is a variable-width character encoding used for electronic communication. Defined by the Unicode Standard, the name is derived from Unicode (or **Universal Coded Character Set) Transformation Format – 8-bit.**
  *  backward compatibility with ASCII: the first 128 characters of Unicode, which correspond one-to-one with ASCII,
## DNS - Domain Name System
  * A web URL is essentially an alias for an IP address (or many ip Addresses) that requests can be routed to.
  * The dot at the end of an URL is the root. example: `www.google.com.`
  * Resolving Name Server, Root Name Server, TLD Name Server, Authoritative Name.
### DNS Record Types
  * `nslookup` command enters editor
  * `set type=` command set's the type of record.
    * example: `set type=A` sets to A
  * `A`: most common; map a hostnames to IP address (IPv4, 32-bit address)
  * `NS`: Name Server that is responsible for a DNS zone
  * `MX`: Mail Exchange record specifies where email gets sent to
  * `CNAME`: Canonical Name, an alias for another hostname
  * `AAAA`: similar to A, but uses IPv6, 128-bit address
### DNS Providers
  * Examples of DNS Providers
    * Amazon Route 53
    * CloudFlare
    * Verisign
    * EasyDNS
    * Azure DNS
### DNS Resolution
Notice that there were four request-response stages,
  1. Starting the journey at the `root name servers`
  2. continuing to the .com top `level domain (TLD)`
  3. followed by the google.com `Name Servers (NS)`
  4. concluded with fifteen (!) `Address Records (A)`
### `http` module
  * The Node.js framework can be used to develop web servers using the `'http'` module. The application can be made to *listen on a particular port and send a response* to the client whenever a request is made to the application.
  * The `'request'` *module can be used to get information from web sites*. The information would contain the entire content of the web page requested from the relevant web site.
### Express Framework
  * minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications
  * not node native, need to install module using `npm i express`
  * provides us with additional functionality to more easily build web apps
### URI - Uniform Resource Identifier
  * sequence of characters that distinguishes one resource from another.
### Template Engine
  * Template Engines are tools that help us break HTML code into smaller pieces.
  * we can reuse across multiple HTML files. 
  * feed data into variables that help you simplify your code. 
  * You can only use template engines if you had a way to compile them into HTML.
### EJS Template Engine - Embedded Javascript Templates
  * Templating language that lets you generate HTML markup with plain JavaScript.
  * server side rendering
    * example function flow: res.render -> html -> browser
    * `<%= %> syntax`, tells EJS that we want the result of this code to show up on our page