# Collections

## What is Collections ?

---

***Collection classes are specialized classes for data storage and retrieval. These classes provide support for stacks, queues, lists, and hash tables. Most collection classes implement the same interfaces.***

***Collection classes serve various purposes, such as allocating memory dynamically to elements and accessing a list of items on the basis of an index etc. These classes create collections of objects of the Object class, which is the base class for all data types in C#.***


 ***Collection is a class , so you must declare an instance of the class before you can add elements to that collection.***

 ---

## Example on a Collection :

 ---

 ```

// Create a list of strings.
var salmons = new List<string>();
salmons.Add("chinook");
salmons.Add("coho");
salmons.Add("pink");
salmons.Add("sockeye");

// Iterate through the list.
foreach (var salmon in salmons)
{
    Console.Write(salmon + " ");
}
// Output: chinook coho pink sockeye


 ```


***The example uses the generic List<T> class, which enables you to work with a strongly typed list of objects.***


 ---

## Kinds of Collections

 ---


***Many common collections are provided by .NET. Each type of collection is designed for a specific purpose .***


**Kinds of collections :**


- **System.Collections.Generic** *classes* : ***generic collection is useful when every item in the collection has the same data type. A generic collection enforces strong typing by allowing only the desired data type to be added.***


- **System.Collections.Concurrent** *classes* : ***provide efficient thread-safe operations for accessing collection items from multiple threads.***


- **System.Collections** *classes* : ***do not store elements as specifically typed objects, but as objects of type ```Object```.***

---


# Enumeration types

## What is Enumeration ?

---

***An ```enum``` is a special "class" that represents a group of constants (unchangeable/read-only variables).***

---

## Example of enum :

---

```
enum Level 
{
  Low,
  Medium,
  High
}

```


***You can access ```enum``` items with the **dot** syntax :***


```

Level myVar = Level.Medium;
Console.WriteLine(myVar);

```


***By default, the associated constant values of enum members are of type integer ; they start with zero and increase by one following the definition text order. You can explicitly specify any other integral numeric type as an underlying type of an enumeration type. You can also explicitly specify the associated constant values, as the following example shows :***


```


enum ErrorCode : ushort
{
    None = 0,
    Unknown = 1,
    ConnectionLost = 100,
    OutlierReading = 200
}


```

---

## Uses of Enumeration:

---

***assign the names or string values to integral constants, that make a program easy to read and maintain.***

---
