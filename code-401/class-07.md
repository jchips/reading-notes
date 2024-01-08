# Reading Notes 7

This topic is important because bearer authentication is secure authentication and is commonly used. It allows users to safely and securely log in and out of sites that we make.

## Intro to JWT

What is a JSON Web Token (JWT)?

- "A JSON Web Token (JWT) is a compact, URL-safe means of representing claims between two parties. It is often used for authentication and authorization purposes in web development. A JWT is a string that consists of three parts: a header, a payload, and a signature. These parts are separated by dots." - ChatGPT

When should we use JSON Web Tokens?

- We should use JWTs for authorization of information exchange.

Claims are expected in which structural component of a JWT?

- It consists of three parts: a header, a payload, and a signature, all separated by dots. It typically looks like: `xxxxx.yyyyy.zzzzz`

Source: ChatGPT & <https://jwt.io/introduction/>

## Are JWTs Secure?

If I get a JWT and I can decode the payload, how can we call that secure?

- The JWT creates a signature out of the encrypted payload and a secret key. If someone doesn't have both of those things, then the token will fail its verification.

If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

- The payload and the secret.

Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

- You can imagine that the concatenated content is a message and the secret is something needed to read to the message. So, to send this information, you would encrypt the message so only the person who has the secret can read it. By doing this, you are signing it so that it the reciever can only read your message if they have the secret (and the message itself).

Source: <https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure>

## JWTs Explained

Why use JWT?

- It is used to securely transfer information between two bodies (users, servers, etc.). They are digitally signed, so the information is verified and trusted.

JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

- This is useful because it makes it easy to send. You can send it as a GET request (URL) or POST request (HTTP header), and it's fast. The JWT self-contains information about the user.

What are the three components (the structure) of a JWT signature?

- A JWT consists of three parts: a header, a payload, and a signature, all separated by dots. It typically looks like: `xxxxx.yyyyy.zzzzz`.

Source: <https://www.youtube.com/watch?v=926mknSW9Lo>

## Reflection

- My learning goals for this class are understanding bearer authentication better.

## Things I want to know more about
