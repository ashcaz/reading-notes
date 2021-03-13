# Hashtables

**LINKS**

- [Intro to Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- [Video: What is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
- [Basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- [Hash table wiki](https://en.wikipedia.org/wiki/Hash_table)

## What is a Hashtable?

Terminology:

1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
2. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Why do we use them?

1. Hold unique values
2. Dictionary
3. Library

## What are they?

Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

Since we are able to hash our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. This is ideal when quick lookups are required.
[Back to Homepage](https://ashcaz.github.io/reading-notes)
