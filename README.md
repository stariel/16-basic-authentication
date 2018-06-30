https://travis-ci.com/stariel/16-basic-authentication/jobs/132216616
 16: Basic Auth
===

## Server Endpoints
### `/api/signup`
* `POST` request
* the client should pass the username, email and password in the body of the request
* the server should respond with a token (generated using `jwt`)
* the server should respond with **400 Bad Request** to a failed request

### `/api/signin`
* `GET` request
* the client should pass the username and password to the server using a `Basic:` authorization header
* use middleware to parse the auth header for username/password
* perform some basic validation
* the server should respond with a token for authenticated users
* the server should respond with **401 Unauthorized** for non-authenticated users
