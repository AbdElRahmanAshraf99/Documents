<h3 id="q1"> 1. What is HTTP?</h3>
<details>
<summary>Answer</summary>

- HTTP (Hypertext Transfer Protocol) is a set of rules which is used for transferring files on the WWW (World Wide Web).
- HTTP doesn't have any security.

</details>

<h3 id="q2"> 2. What is HTTP Request?</h3>
<details>
<summary>Answer</summary>

- HTTP Requests are messages which are sent by the client or user to initiate an action on the server.
- HTTP Request consists of various things:
  - Request Line. (GET /index.html HTTP/1.1)
  - The recourse identified by a request.
  - Request header fields.

</details>

<h3 id="q3"> 3. What are HTTP Methods?</h3>
<details>
<summary>Answer</summary>

- GET
  - retrieves information from the given server using the given URI.
- POST
  - sends data to the server.
- HEAD
  - returns headers only for checking resource existence, modifications, or size without downloading content.
- PUT
  - replaces all the current representation of the target resource with the uploaded content.
- DELETE
  - removes all the current representations of the target resource, which is given by URI.
- CONNECT
  - establishes a tunnel to the server, which is identified by a given URI.

</details>

<h3 id="q4"> 4. What is the status code?</h3>
<details>
<summary>Answer</summary>

- The server issues an HTTP status code in response.
- Status code is a 3-digit integer. The first digit of status code is used to specify one of five standard classes of responses. The last two digits
  of
  status code don't have any categorization role.
- 1xx => Informational
- 2xx => Success
- 3xx => Redirection
- 4xx => Client Error
- 5xx => Server Error

</details>

<h3 id="q5"> 5. What are Persistent Connections?</h3>
<details>
<summary>Answer</summary>

- In HTTP/1.0, the connection is closed after a single request or response pair.
- In HTTP/1.1, There is a new mechanism, which is known as keep-alive mechanism.
- In this mechanism, a connection could be reused for more than one request.

</details>

<h3 id="q6"> 6. What is HTTP Response?</h3>
<details>
<summary>Answer</summary>

- HTTP response sent by a server to the client.
- It is used to provide response to client with the resource it requested.
- It contains the following things:
  - Status Line
  - Response header fields
  - Message body

</details>

<h3 id="q7"> 7. How to secure HTTP connection?</h3>
<details>
<summary>Answer</summary>

1. HTTPS
   - It is the secure version of HTTP, which communications between client and server are encrypted using TLS (Transport Layer Security).
   - It uses SSL/TLS to encrypt data before it's sent over the network, it can't be read by unauthorized parties.

2. HSTS

   - It is a security policy mechanism that helps to protect websites against man-in-the-middle attacks such as protocol downgrade attacks and cookie
     hijacking.
   - The server sets an HSTS policy in the browser through a response header, which forces the browser to only interact with the server over HTTPS
     for a specified period.

3. Secure HTTP Headers

   - Content Security Policy (CSP)
     - allows you to restrict the sources from which the browser can load resources.
     - helps prevent XSS attacks by specifying which content is allowed to execute on a webpage.
   - X-Content-Type Options
     - prevents browsers from MIME-sniffing a response away from the declared content-type.
     - reduces the risk of certain types of attacks like XSS attacks.
   - X-Frame Options
     - controls whether a browser should be allowed to render a page in a `<iframe>`, `<frame>`, `<object>`, or `<embed>` tag.
     - helps to prevent clickjacking attacks.

4. Authentication and Authorization

   - OAuth
     - is an open standard for access delegation, commonly used as a way to grant applications limited access to user information without exposing
       passwords.
   - JWT (JSON Web Token)
     - is a compact,URL-safe means of representing claims to be transferred between two parties often used for authentication and information
       exchange.
   - Basic and Digest Authentication
     - Basic sends user credentials in an encoded form, while Digest sends a hashed version of credentials.

5. Secure Cookies

   - Secure Attribute
     - ensures that cookies are only sent over HTTPS connections.
   - HTTPOnly Attribute
     - prevents client-side scripting from accessing the cookies, mitigating XSS attacks.
   - SameSite Attribute
     - prevents the browser from sending the cookies along with cross-site requests, helping to protect against CSRF attacks.

6. Data Encryption

   - End-to-End Encryption
   - Database Encryption

7. Web Applications Firewall
   - It protects web applications by filtering and monitoring HTTP traffic between a web application and the Internet.
</details>
