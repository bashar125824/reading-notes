# What is Interfaces ?

---

![IMG](https://i.stack.imgur.com/0xtVd.png)

---

***A blueprint of a class . It is like abstract class because all the methods which are declared inside the interface are abstract methods. It cannot have method body and cannot be instantiated. It is used to achieve multiple inheritance which can't be achieved by class .***

***By using interfaces, you can, for example, include behavior from multiple sources in a class. That capability is important in C# because the language doesn't support multiple inheritance of classes. In addition, you must use an interface if you want to simulate inheritance for structs, because they can't actually inherit from another struct or class .***

***Interface may define default implementations for some or all of its members. A class or struct that implements the interface doesn't have to implement members that have default implementations. For more information, see default interface methods .***

***An interface defines a contract. Any class or struct that implements that contract must provide an implementation of the members defined in the interface .***


***Interfaces are always implemented by more than one class .***

---

## How to define an interface ?

---

***You define an interface by using the **interface** keyword as the following example shows :***


```

interface IEquatable<T>
{
    bool Equals(T obj);
}

```

---

## Implemintation of an interface :

---

```
interface ISampleInterface
{
    void SampleMethod();
}

class ImplementationClass : ISampleInterface
{
    // Explicit interface member implementation:
    void ISampleInterface.SampleMethod()
    {
        // Method implementation.
    }

    static void Main()
    {
        // Declare an interface instance.
        ISampleInterface obj = new ImplementationClass();

        // Call the member.
        obj.SampleMethod();
    }
}

```

---


## What problem does the interface solve?

---

***The basic problem an interface is trying to solve is to **separate how we use something from how it is implemented.*****

---



