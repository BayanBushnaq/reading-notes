# Hashtables

## What is a Hashtable?
#### A hash table is a data structure that you can use to store data in key-value format with direct access to its items in constant time. Hash tables are said to be associative, which means that for each key, data occurs at most once.


#### Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

#### The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

#### Since we are able to hash our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. This is ideal when quick lookups are required.


### Creating a Hash
#### A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a simplistic hashing algorithm:

-  Add or multiply all the ASCII values together.
- Multiply it by a prime number such as 599.
- Use modulo to get the remainder of the result, when divided by the total size of the array.
- Insert into the array at that index.


### Collisions
#### A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.

### What would happen if two different keys resolved to be the same index of the array? 
#### This is called a collision. The hash map needs to be able to handle two keys resolving to the same index.

#### If two keys ever ultimately resolved to the same index, then two calls to .Add(key, val) with different keys would overwrite each other.

#### Collisions are solved by changing the initial state of the buckets. Instead of starting them all as null we can initialize a LinkedList in each one! Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list. Each index in the array is called a “bucket” because it can store multiple key/value pairs.

#### Since different keys can lead to the same bucket it’s important to store the entire key/value pair in the bucket, not just the value. The key must be stored with the value! If only values were stored in buckets then it would be impossible to determine which value to return when a key led you to a bucket.

### Hash maps do this to store values:

- accept a key
#### calculate the hash of the key
#### use modulus to convert the hash into an array index
#### store the key with the value by appending both to the end of a linked list
- Hash maps do this to read value:

#### accept a key
#### calculate the hash of the key
#### use modulus to convert the hash into an array index
#### use the array index to access the short LinkedList representing a bucket
#### search through the bucket looking for a node with a key/value pair that #### matches the key you were given

### Methods
- set()
#### When adding a new key/value pair to a hashtable:

#### send the key to the hash() method.
#### Once you determine the index of where it should be placed, go to that index
#### Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
#### If something does exist, add the new key/value pair to the data structure within that bucket.
- get()
#### The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

- has()
#### The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

- keys()
#### The keys() method returns a collection (array) of unique hash keys.

- hash()
#### The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.