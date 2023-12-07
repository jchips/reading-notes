# Reading Notes 6

Today's topic is important to understand basic authentication so I can use it in my projects and then start learning more advanced authentication. Authentication is really common and important for applications in this day and age.

## Securing Passwords

1. Explain to a non-technical friend how you would safely hash and store a password.

    I would encrpyt the password into code so the password can only be understood by the computer. Then, I would save that in storage and compare it to a typed password that a user inputs. If it matches the decoded encrypted password, then the user can log in. Otherwise, they can't.

2. What is Bcrypt?

    Bcrypt is an adaptive hash function.

3. Why might you use something like Bcrypt?

    You would use Bcrpyt to hash your password.

Source: <https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html>

## Basic Auth

1. What is Basic Authentication?

    Basic authentication is when a web browswer asks for a username and password when making a request.

2. What properties are necessary in the header of a Basic Auth request?

    Needed in the header of a Basic Auth request is `Authorization: Basic <credentials>` where the credentials is a unique key given to you.

3. How are username:password in Basic Auth encoded?

    "If the browser uses Aladdin as the username and open sesame as the password, then the field's value is the Base64 encoding of Aladdin:open sesame, or QWxhZGRpbjpvcGVuIHNlc2FtZQ==. Then the Authorization header field will appear as 'Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ=='"

Source: <https://en.wikipedia.org/wiki/Basic_access_authentication>

## OWASP auth cheatsheet

1. Define the authentication process to a non-technical recruiter.

    For the authentication process, first a user enters their username. Then, they enter their password. Then those are submitted to the server for verification. If both are valid, then the user is authenticated, and they can gain access to pages they didn't have access to before.

2. How should your error messaging respond (both HTTP and HTML)? Why?

    There should be error messages from the application for the user ID or password being incorrect, the account not existing, or the account being locked or disabled. This is too not confuse the user and make it clear what was wrong with their login attempt.

Source: <https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html#introduction>

## Additional Questions

1. I am most looking forward to learning more basic authentication and to learn stacks and queues.
2. My learning goal is to learn all the basics in authentication.

## Things I want to know more about
