# APIs.

### 1-What does REST stand for?
#### Representational State Transfer (REST) 

### 2- REST APIs are designed around a ____.
#### around resources.

### 3- What is an identifier of a resource? Give an example.
#### A resource has an identifier, which is a URI that uniquely identifies that resource. 
#### For example, the URI for a particular customer order might be:

#### HTTP
#### https://adventure-works.com/orders/1

### 4- What are the most common HTTP verbs?
#### The most common operations are GET, POST, PUT, PATCH, and DELETE.

### 5- What should the URIs be based on?
####  URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

### 6- Give an example of a good URI.
#### https://adventure-works.com/orders 

### 7- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
#### Chatty API is one that requires consumer to make tremendous (subjective matter) amount of distinct API calls to get needed information about a resource.
#### try to avoid "chatty" web APIs that expose a large number of small resources.

### 8- What status code does a successful GET request return?
####  HTTP status code: 200 (OK)

### 9- What status code does an unsuccessful GET request return?
####  404 (Not Found).

### 10- What status code does a successful POST request return?
#### HTTP status code: 201 (Created).

### 11- What status code does a successful DELETE request return?
#### HTTP status code :204 (No Content)
