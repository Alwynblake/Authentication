# Authentication
Fix and document a (broken) Basic Authentication server, with signup and signin capabilities, using a Mongo database for storage.

# Authors: Alistair Blake, Matthew Heyert
# LAB: Authentication

Fixed and documentd a (broken) Basic Authentication server, with signup and signin capabilities, using a Mongo database for storage.


### Assignment: Auth Server
* Create a UML diagram of the authentication system on a whiteboard
* Identify and fix any bugs
* **NEW CODE:** Protect the `/book` and `/book/:id` routes by requiring user authentication
* Document and publish the code with JSDoc

### Testing
* POST to /signup to create a new user
* POST to /signin to login as a user (use basic auth)
* Tests for auth middleware and the routes
  * Send it a basic header
  * Routes assert the requirements (signup/signin)
  * The book routes protected properly

### Notes

Signup with httpie: 
```
echo '{"username":"name","password":"pass"}' | http post :3000/signup
```
Signin with httpie: 
```
http post :3000/signin -a username:password
```

## Assignment Submission Instructions
Refer to the the [lab submission instructions](../../../reference/submission-instructions/labs/README.md) for the complete lab submission process and expectations


