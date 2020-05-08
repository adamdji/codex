<!-- omit in toc -->
# HTTP

<!-- omit in toc -->
## Index

- [Methods](#methods)
- [Codes](#codes)
  - [200](#200)
  - [300](#300)
  - [400](#400)
  - [500](#500)
- [Headers](#headers)
- [CORS](#cors)

---

## Methods

- `GET`: Request representation of the specififed resource
- `HEAD`: `GET` with no body
- `POST`: Submit an entity to the specified resource
- `PUT`: Replace all current representations of the target resource with the request payload
- `DELETE`: Deletes the specified resource
- `OPTIONS`: Describe communication options for the target resource
- `PATCH`: Apply partial modifications to a resource

---

## [Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

### 200

- `201 Created`: New resource has been created, typically sent after `POST`
- `206 Partial Resource`: When the `Range` header is sent from the client to request only part of a resource

### 300

- `300 Multiple Choice`: UA should choose which response (user chooses)
- `301 Moved Permanently`: New URL is given in the response
- `307 Temporary Redirect`: Same HTTP Method used
- `308 Permanent Redirect`: Same semantics as 301 but UA must not change HTTP method used

### 400

- `400 Bad Request`
- `401 Unauthorized`
- `403 Forbidden`: Client is known, but not authorized to access the requested resource
- `404 Not Found`
- `405 Method Not Allowed`
- `409 Conflict`: Request conflicts with current state of the server
- `410 Gone`: Requested content has been permanently deleted, limited time use
- `411 Length Required`: `Content-Length` header is not defined and server needs it
- `413 Payload Too Large`: Requested entity is larger than limits defined by server.
- `414 URI Too Long`
- `415 Unsupported Media Type`: Media format of the requested data is not supported.
- `418 I'm a teapot`

### 500

- `500 Internal Server Error`
- `501 Not Implemented`: Requested method is not supported and cannot be handled
- `502 Bad Gateway`: Server, while working as a gateway to get a response, could not get a response
- `503 Service Unavailable`: Server is not ready to handle the request (Maintenance) `Retry-After` header useful
- `504 Gateway Timeout`: Gateway server could not get a response

---

## Headers

<!-- omit in toc -->
### Authentication

- `WWW-Authenticate`: Defines authentication method that should be used to access a re source
- `Authorization`: Credentials to authenticate a UA with server

<!-- omit in toc -->
### Caching

-`Expires`: Date/time after which the response is considered stale
-`Clear-Site-Date`: Clears browsing data associated with the requesting website

<!-- omit in toc -->
### Conditionals

-`Last-Modified`: Last modification date of the resource
-`ETag`: Unique string identifying the version of the resource
-`If-Modified-Since`: Request conditional, only transmitted if it has been modified after the given date
-`If-Unmodified-Since`: Reverse of previous

<!-- omit in toc -->
### Connection Management

-`Connection`: Controls whether the network connection stays open a fter the current transaction finishes
-`Keep-Alive`: Controls how long a persistent connection should stay open

<!-- omit in toc -->
### Content Negotiation

---

## CORS