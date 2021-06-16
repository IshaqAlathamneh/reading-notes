# Hash Table
A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found


1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
1. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
1. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

### Complexity
Because we know the index of the information we want we can access that information in O(1) time.

### Creating a Hash
Here is a possible suggestion:

1. Add or multiply all the ASCII values together.
1. Multiply it by a prime number such as 599.
1. Use modulo to get the remainder of the result, when divided by the total size of the array.
1. Insert into the array at that index.

Example: 
```
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 
```

### Internal Methods
1. Add()
When adding a new key/value pair to a hashtable.
1. Find()
The Find takes in a key, gets the Hash.
1. Contains()
The Contains method will accept a key, and return a bool on if that key exists inside the hashtable.
1. GetHash()
The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.