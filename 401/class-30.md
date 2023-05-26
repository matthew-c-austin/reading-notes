# Hash Tables Cheatsheet

[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[What is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)

[Basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

[Hash table wiki](https://en.wikipedia.org/wiki/Hash_table)

## Terminology

- **Hash**: A function that converts one value to another. Hash functions in hash tables are used to convert keys into array indices.
- **Hash Table**: A data structure that uses hash functions to map keys to values.
- **Key**: An item that has a unique identifier.
- **Value**: The data associated with a key.
- **Collision**: Occurs when two different keys hash to the same index in an array.

## Types of Hash Tables

- **Open Addressing**: A collision-resolution strategy that finds the next open slot or address in the hash table for inserting a value whenever a collision occurs.
- **Separate Chaining**: A collision-resolution strategy where each element of the hash table's internal array is a linked list or another hash table itself.

## Adding a Key-Value Pair to a Hash Table

1. Compute the hash code of the key, which will often be an integer.
2. Modulo that hash code by the length of the internal array (the modulo operation will make sure that the result fits within the boundaries of the array).
3. If the computed index in the array is unoccupied, insert the value there.
4. If a collision occurs, resolve it using a collision-resolution strategy (either open addressing or separate chaining).

## Hash Table Methods

- **set()**: Adds a new key/value pair to a hashtable.
- **get()**: Takes in a key, gets the hash, and goes to the index location specified. Once at the index location in the array, it iterates through the bucket to see if the key exists and return the value.
- **has()**: Accepts a key and returns a boolean indicating if that key exists inside the hashtable.
- **keys()**: Returns a collection (array) of unique hash keys.
- **hash()**: Accepts a key as a string, conducts the hash, and then returns the index of the array where the key/value should be placed.

## Big O

- Time complexity for inserting:
  - Worst case: O(n) (all keys hash to the same index)
  - Best case: O(1)
  - Average case: O(1)
- Space complexity for inserting: O(n)
- Time complexity for searching:
  - Worst case: O(n) (all keys hash to the same index)
  - Best case: O(1)
  - Average case: O(1)
- Space complexity for searching:
  - Worst case: O(n)
  - Best case: O(1)
  - Average case: O(1)
  