# What is OOP ?

---

***object-oriented programming : is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.***

***OOP focuses on the objects that developers want to manipulate rather than the logic required to manipulate them. This approach to programming is well-suited for programs that are large, complex and actively updated or maintained. This includes programs for manufacturing and design, as well as mobile applications; for example, OOP can be used for manufacturing system simulation software.***

---

**There is three primary characteristics of object-oriented programming :**

---

- *Inheritance* 

- *Encapsulation*

- *Polymorphism*

---


# Inheritance

---

***It is a mechanism where you can to derive a class from another class for a hierarchy of classes that share a set of attributes and methods.***


***The class whose members are inherited is called the **base** class, and the class that inherits those members is called the **derived** class.***


---

## Abstract and virtual methods

---


***When a base class declares a method as virtual, a derived class can override the method with its own implementation. If a base class declares a member as abstract, that method must be overridden in any non-abstract class that directly inherits from that class***.

---

## Interfaces

---

***is a reference type that defines a set of members.***

---

## Differences Between Interfaces and Abstract Classes :

---

**Abstract class** : *allows you to create functionality that subclasses can implement or override*

**Interface** : *only allows you to define functionality, not implement it*

---

## Abstract Classes and Class Members :

---

***Classes can be declared as abstract by putting the keyword **abstract** before the class definition. For example :***

```

public abstract class A
{
    // Class members here.
}

```


***An abstract class cannot be instantiated. The purpose of an abstract class is to provide a common definition of a base class that multiple derived classes can share. For example, a class library may define an abstract class that is used as a parameter to many of its functions, and require programmers using that library to provide their own implementation of the class by creating a derived class.***


---

## Sealed Classes and Class Members :

---

***Classes can be declared as sealed by putting the keyword sealed before the class definition. For example:***

```

public sealed class D
{
    // Class members here.
}

```

***A sealed class cannot be used as a base class. For this reason, it cannot also be an abstract class. Sealed classes prevent derivation. Because they can never be used as a base class, some run-time optimizations can make calling sealed class members slightly faster.***


---


# Polymorphism

---

***Describes situations in which something occurs in several different forms. In computer science, it describes the concept that you can access objects of different types through the same interface.***


***It has two distinct aspects:***

- **At run time, objects of a derived class may be treated as objects of a base class in places such as method parameters and collections or arrays. When this polymorphism occurs, the object's declared type is no longer identical to its run-time type.**

- **Base classes may define and implement virtual methods, and derived classes can override them, which means they provide their own definition and implementation. At run-time, when client code calls the method, the CLR looks up the run-time type of the object, and invokes that override of the virtual method. In your source code you can call a method on a base class, and cause a derived class's version of the method to be executed.**

---

## Virtual members

---

***When a derived class inherits from a base class, it gains all the methods, fields, properties, and events of the base class. The designer of the derived class has different choices for the behavior of virtual methods:***

- **The derived class may override virtual members in the base class, defining new behavior.**

- **The derived class may inherit the closest base class method without overriding it, preserving the existing behavior but enabling further derived classes to override the method.**


- **The derived class may define new non-virtual implementation of those members that hide the base class implementations.**

---







