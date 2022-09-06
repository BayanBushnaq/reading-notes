# CRUD
---------------------------------------------------------------------------------------------------------------------------

## In your own words, describe what each group of status code represents:

### 100's = These are informational status codes.
### 200's = These are the success codes.
### 300's = These are redirection codes. 
### 400's = These are the client error codes.
### 500's = These are the server error codes.

## What is a status code 202? 
### Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.

## What is a status code 308? 
###  Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.
### It’s helpful when we have multiple endpoints for one

## What code would you use if an update didn't return data to a client? 
### 204 No Content

## What code would you use if a resource used to exist but no longer does?
### 410 Gone

## What is the 'Forbidden' status code?
### 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

---------------------------------------------------------------------------------------------------------------------------

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?
### to deploy it . 

## What is middleware?
###  software that provides common services and capabilities to applications outside of what's offered by the operating system

## What does app.use(express.json()) do?
### It parses incoming JSON requests and puts the parsed data in req.

## What does the /:id mean in a route?
### The req. params property is an object containing properties mapped to the named route “parameters”.

## What is the difference between PUT and PATCH?
### PUT is a method of modifying resource where the client sends data that updates the entire resource . 
### PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

## How do you make a default value in a schema?
### a default value for an item using the default keyword. When a data doesn't have a corresponding value,
###  the value of this keyword will be used instead to do the validation checks

## What does a 500 error status code mean?
### means something has gone wrong on the website's server.

## What is the difference between a status 200 and a status 201?
### 200: “Everything is OK.” This is the code that is delivered when a web page or resource acts exactly the way it's expected to.
### 201: “Created.” The server has fulfilled the browser's request, and as a result, has created a new resource.
