# Hash Tables

![](https://miro.medium.com/max/315/1*nzISDLbkF67C-BTQtFc_DQ.png)

## What is a Hashtable?

is a data structure containing an unordered collection of keys that are mapped to values using hashing.

## Properties

Key/Value
When using hashmaps, data is stored in the form of key/value pairs. The key, used to reference the data, can be any data type. Yes, even an object or an array can be a key when using a hashmap! Similarly, values in hashmaps are allowed to be null.

## Hashing

Hashing is a term used to describe the manipulation of a string or input key, and representing it with a hash value. This hash value is typically determined by an algorithm or hash function.

## Hashing functions

 are used to return indexes in the array where the value will be stored. Hashing functions take keys as inputs and return an index with the hashmap’s array. Hashing functions are deterministic, meaning the hashing function always returns the same index when provided the same key. Hashing functions must be predictable and consistent to retrieve the stored value via the key. A good hash function should be efficient and assign unique keys.

 ## Collisions

 occurs when multiple keys hash to the same index. This is a situation in which two or more keys produce the same hash value, subsequently occupying the same array index. When this happens, you need to make sure that you can differentiate between conflicting keys.

## separate chaining 

is one way to resolve this. This happens by storing multiple key-value pairs at the index in question. In this situation, you store all the key-pairs that collide in a linked-list and parse through them.


![](https://res.cloudinary.com/practicaldev/image/fetch/s--dsm7QIAp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://i.imgur.com/qJJCDf1.png)

Terminology :

####

1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

2. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.



[Github view](https://github.com/sbkhaloof/growthmindsit)
