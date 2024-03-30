# Homework #12
In this homework assignment, we continue to refine our REST API application from [homework #11](https://github.com/Goit-Home-Works/Py_WEB_11).

## Tasks
Implement authentication mechanism in the application.
Implement authorization mechanism using JWT tokens so that all operations with contacts are performed only by registered users.
Users should have access only to their own contact operations.
## General Requirements
During registration, if a user already exists with such an email, the server returns an HTTP 409 Conflict error.
The server hashes the password and does not store it in plaintext in the database.
Upon successful registration, the server should return an HTTP status response of 201 Created and the data of the new user.
For all POST operations to create a new resource, the server returns a status of 201 Created.
During the POST operation for authentication, the server accepts a request with user data (email, password) in the request body.
If the user does not exist or the password does not match, an HTTP 401 Unauthorized error is returned.
The authorization mechanism using JWT tokens is implemented with a pair of tokens: an access token and a refresh token.

## Execution

To run the program, copy and paste the following command into your terminal:

```bash
python3 src/main.py
```

After that, click on API DOC button.