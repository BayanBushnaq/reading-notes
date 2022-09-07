# Authentication
## What is OAuth?
### OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial,
### related, single logon credential.

## Give an example of what using OAuth would look like.
### when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.
### You then click on the button linked to the other website, the other website authenticates you,
### and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

## How does OAuth work? What are the steps that it takes to authenticate the user?
### 1- Identification. Users have to prove who they are.
### 2- Authentication. Users have to prove they are who they say they are.
### 3- Authorization. Users have to prove they're allowed to do what they are trying to do.

## What is OpenID?
### is about authentication , its used for humans logging into machines.


------------------------------------------------------------------

## What is the difference between authorization and authentication?
###  Authentication verifies the identity of a user or service.
###  Authorization determines their access rights.

## What is Authorization Code Flow?
### Authorization code flow is used to obtain an access token to authorize API requests. 
### Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API.
## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

## What is Implicit Flow with Form Post?
### As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow,
### which is intended for Public Clients, or applications which are unable to securely store Client Secrets.


## What is Client Credentials Flow?
### Client creadentials Flow happened With machine-to-machine (M2M) applications the system authenticates and authorizes the app rather than a user.

## What is Device Authorization Flow?
### Type of authorization happen With input-constrained devices that connect to the internet, rather than authenticate the user directly,
### the device asks the user to go to a link on their computer or smartphone and authorize the device.

## What is Resource Owner Password Flow?
### which requests that users provide credentials (username and password), typically using an interactive form.
