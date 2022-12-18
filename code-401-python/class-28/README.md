# What is JSON Web Token?
## JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

## Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

## When should you use JSON Web Tokens?
### Authorization: This is the most common scenario for using JWT.
### Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties.

## What is the JSON Web Token structure?
### In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

 - ![Auth0](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT6WE6QPviUVA7jpM4wXWjwaauKzsSuDEYWFw&usqp=CAU)

## How do JSON Web Tokens work?
### In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

## How JWT Works?

### The JWT is just an authorization token that should be included in all requests:
 - The JWT is acquired by exchanging an username + password for an access token and an refresh token.

 - The access token is usually short-lived (expires in 5 min or so, can be customized though).

 - The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.