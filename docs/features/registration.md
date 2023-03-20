---
sidebar_position: 1
---

# Registration

In order to control the registration process, we created two tables:

- user_candidates
- users

When a user comes to our application and wants to register, they only enter an email address.

Then we create a _user candidate_ record with a randomly created secret and send a mail with this secret.

When users clicks that link, they will be redirected to a page where they will enter their name and password.

User submits this form and we create a record in _users_ table.

In the first step, user candidate request will be sent to: _/api/auth/signupcandidate_

In the second step, user request will be sent to: _/api/auth/signup_

Thus, we secure the email addresses from abusive attackers.
