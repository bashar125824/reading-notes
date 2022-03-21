# Classes

---

***A class is a user-defined blueprint or prototype from which objects are created. Basically, a class combines the fields and methods(member function which defines actions) into a single unit. In C#, classes support polymorphism, inheritance and also provide the concept of derived classes and base classes .***

***Classes considered as Reference type .***

---

- **Declaration of class**

***Generally, a class declaration contains only a keyword **class** , followed by an identifier(name) of the class. But there are some optional attributes that can be used with class declaration according to the application requirement***

***Example of Declaring a class :***

```

//[access modifier] - [class] - [identifier]
public class Customer
{
   // Fields, properties, methods and events go here...
}

```

---

- **Creating objects**

---

***a class and an object are different things. A class defines a type of object, but it is not an object itself. An object is a concrete entity based on a class, and is sometimes referred to as an instance of a class.***

***Example of Creating an object :***

```
Customer object1 = new Customer();

```

---

- **Class inheritance**

---

***In C#, it is possible to inherit fields and methods from one class to another. We group the "inheritance concept" into two categories:***

- ***Derived Class (child) - the class that inherits from another class***
- ***Base Class (parent) - the class being inherited from***

---

# Constructors

---

***A special method of the class that is automatically invoked when an instance of the class is created .***

---

***The main use of constructors is to initialize the private fields of the class while creating an instance for the class.***

---

***When you have not created a constructor in the class, the compiler will automatically create a default constructor of the class. The default constructor initializes all numeric fields in the class to zero and all string and object fields to null.***

---

- **Constructor Syntax**

---

***A constructor is a method whose name is the same as the name of its type .***

---

- **Static Constructor**

***used to initialize any static data, or to perform a particular action that needs to be performed only once .***

***it is called automatically before the first instance is created or any static members are referenced.***

---

# Properties

---

***a member of a class that provides a flexible mechanism for classes to expose private fields .***

***enable a class to expose a public way of getting and setting values, while hiding implementation or verification code.***

---

- **Properties with backing fields**

***get* accessor returns the value of the private field , and the *set8 accessor may perform some data validation before assigning a value to the private field .**

---

# Fundamentals of garbage collection

---

***A core computer science concept which is a process for automatic memory management.***

---

***The C language provides several functions for handling memory allocation and management. The most used are:***

- ***malloc — This function allocates memory and leaves the memory uninitialized.***
- ***free — This function releases a block of memory specified by address.***
- ***calloc— This function allocates memory and initializes all bits to zero.***
- ***dealloc — This function re-allocates memory extending it up to new size.***

---

- **Benefits**

---

***Garbage collection, used the right way, can make a developer’s life easier when it comes to memory management. When you’re done with some code, the memory occupied by this code will automatically be cleaned up.***

---

# Stack and Heap

***Stack Memory :***

1. **It is an array of memory.**

2. **It is a LIFO (Last In First Out) data structure.**

3. **n it data can be added to and deleted only from the top of it.**

---

***Heap Memory***

1. **It is an area of memory where chunks are allocated to store certain kinds of data objects.**

2. **In it data can be stored and removed in any order.**








