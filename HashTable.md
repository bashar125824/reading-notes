# Hash Table

## What is Hashing ?

***Hashing is a technique to convert a range of key values into a range of indexes of an array. We're going to use modulo operator to get a range of key values. Consider an example of hash table of size 20, and the following items are to be stored. Item are in the (key,value) format.***

![IMG](https://www.tutorialspoint.com/data_structures_algorithms/images/hash_function.jpg)

(1,20)
(2,70)
(42,80)
(4,25)
(12,44)
(14,32)
(17,11)
(13,78)
(37,98)

| Sr.No. | 	Key	    |     Hash	    |     Array Index |
|--------|----------|---------------|-----------------|
|  1	   |    1	    |   1 % 20 = 1	|         1       |
|  2	   |    2	    |   2 % 20 = 2	|         2       |
|  3	   |    42	  |   42 % 20 = 2 |         2       |
|  4	   |    4	    |   4 % 20 = 4	|         4       |
|  5	   |   12	    |   12 % 20 = 12|	        12      |
|  6	   |   14	    |   14 % 20 = 14|	        14      |
|  7	   |   17     |   17 % 20 = 17|         17      |
|  8     |   13	    |   13 % 20 = 13|         13      |
|  9  	 |   37	    |   37 % 20 = 17|         17      |


# What is Hash Table ?

***Hash Table is a data structure which stores data in an associative manner. In a hash table, data is stored in an array format, where each data value has its own unique index value. Access of data becomes very fast if we know the index of the desired data.***

***Thus, it becomes a data structure in which insertion and search operations are very fast irrespective of the size of the data. Hash Table uses an array as a storage medium and uses hash technique to generate an index where an element is to be inserted or is to be located from.***

## Definitionsto know :

- **Buckets** : ***A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.***

- **Collisions** : ***A collision is what happens when more than one key gets hashed to the same location of the hashtable.***

## Basic Operations

**Search** : ***Searches an element in a hash table***.

**Insert** : ***inserts an element in a hash table***.

**delete** : ***Deletes an element from a hash table***.

## Uses of Hash Tables :

- ***Hold unique values***

- ***Dictionary***

- ***Library***

## Example :

``` ["Greenwood:98103", "Downtown:98101", "Alki Beach:98116", "Bainbridge Island:98110", ...] ```

## Big (O) Notation :

**Space Complexity** : ***O(n)***

**Time Complexity** : ***O(1) in the average*** , and ***O(n) for the worst case***
