---
sidebar_position: 3
---

# Cookie Management

In order to track user's login sessions, we use _sessions_ table.

When user logs in using _/api/auth/signin_, a new record is created in _sessions_ table and the previous records of this user is deleted from the table.

After the login, user receives two tokens: _access token_ and _refresh token_. Access token's lifespan is fairly short comparing to refresh token. The logic is that when the access token expires, user can receive another one using the refresh token, without logging in again. Only after the refresh token expires, user needs to log in.

So when refreshing the access token using refresh token, we check the _sessions_ table and check if there is a record with this user. If there is, we generate new access AND refresh token and lend it to the user.

Out of _sign in_, and _sign up_ routes, all routes needs access token to be send in the request to perform authentication and authorization operations.
