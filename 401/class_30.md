# Hash Tables

## Review, Research, and Discussion

## General

- We use hash tables to hold unique values, as away to store and search for things
- The main idea of a hash table is that it has the ability to store a key into this data structure and quickly retrieve the value. Both are done through hashing.
- The hash function takes a key and returns an interger
- Ability to have a consistent O(1) read and write access

```javascript
  has(key) {
    let LL;
    // 1: hash the key
    let hash = this.hash(key);
    // 2: Get the value of this.map[hash]
    if (this.map[hash]) {
      LL = this.map[hash];
    }
    // 3: Traverse the linked list and find the actual one (because ... collisions)
    let node = LL.head;
    while (node) {
      if (node.value[key]) {
        // 4: Return what we find
        return true;
      }
      node = node.next;
    }
    // 4: Return what we find
    return false;
  }
```

### Creating a hash

- A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:

1. Add or multiply all the ASCII values together.
2. Multiply it by a prime number such as 599.
3. Use modulo to get the remainder of the result, when divided by the total size of the array.
4. Insert into the array at that index.

```text
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 
```

## Terminology

- Hash:
  - A hash is a result of some algorithm which takes a string and converts it into a value that could be used for security or some other purpose.
  - Hash tables utilize this number to determine the index of an array
  
- Buckets:
  - A term to describe what is described in the index of each array. Each index is considered a bucket which means an index may contain multiple key value pairs

- Collisions:
  - When more than one key/value pair gets hashed into the same location/index/BUCKET of the hashtable
