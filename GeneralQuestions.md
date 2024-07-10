### 1. What is the difference between Localstorage and Cookies?

- Both are commonly used for storing data on the client side in web applications, but they serve different purposes and have different
  characteristics that will be discussed below.

#### Purpose

- <strong>LocalStorage:</strong> Used to store data that needs to persist across browser sessions.
- <strong>Cookies:</strong> Used to store data that needs to be sent to the server with every HTTP request.

#### Usage

- <strong>LocalStorage:</strong> Ideal for storing large amounts of data that doesn't need to be sent to
  the server with every request.
- <strong>Cookies:</strong> Commonly used for session management, user tracking, and storing small pieces of data.

#### Access

- <strong>LocalStorage:</strong> Data is accessible only via JavaScript in the browser.
- <strong>Cookies:</strong> Data is accessible via JavaScript and is automatically sent to the server with each HTTP request.

#### Storage Size

- <strong>LocalStorage:</strong> Typically allows for larger storage limits, around 5-10MB per origin.
- <strong>Cookies:</strong> Smaller storage capacity, around 4KB per cookie.

#### Data Persistence

- <strong>LocalStorage:</strong> Data persists even after the browser is closed and reopened, until explicitly deleted.
- <strong>Cookies:</strong> Expiration can be set for each cookie. If no expiration is set, the cookie will expire when the session ends (i.e., when
  the browser is closed).

#### Security

- <strong>LocalStorage:</strong> Data is accessible through JavaScript, which can be a security risk if the site is vulnerable to XSS (Cross-Site
  Scripting) attacks.
- <strong>Cookies:</strong> Cookies can be flagged as 'HttpOnly', making them inaccessible via JavaScript and helping to protect against XSS attacks.


