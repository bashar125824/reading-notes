# What is Stacks and queues ?

***Stacks and Queues are limited access data sturctures .***

***the **Stacks** can be used to maintain a list of operations for an 'undo' function in a piece of software, where the most recent operation is the first to be undone. Stacks are also used to facilitate recursive subroutines where the state of each call is stored in a stack frame and placed on a stack.***


***In operating systems, **Queues** are used to control access to shared resources, such as printers, files and communication lines. Queues are the most appropriate data structure for these examples because: a website cannot service all requests, so it handles them in order of arrival on a first-come-first-served basis.***

---

# Stacks :

***A stack is a conceptual structure consisting of a set of homogeneous elements and is based on the principle of last in first out (LIFO). It is a commonly used abstract data type with two major operations, namely **push** and **pop**. Push and pop are carried out on the topmost element which called **top** , which is the item most recently added to the stack. The push operation adds an element to the stack while the pop operation removes an element from the top position. The stack concept is used in programming and memory organization in computers.***


***A stack is considered to be a restricted data structure as only a limited number of operations are allowed. Besides the push and pop operations, certain implementations may allow for advanced operations such as:***

- **Peek()** :  *View the topmost item in the stack.*

- **Duplicate()** : *Copy the top item’s value into a variable and push it back into the stack.*

- **Swap()** : *Swap the two topmost items in the stack.*

**Rotate()** : *Move the topmost elements in the stack as specified by a number or move in a rotating fashion.*

---

# Queues :

***Queue is an abstract data structure, somewhat similar to Stacks. Unlike stacks, a queue is open at both its ends. One end is always used to insert **(enqueue)** data called **back** and the other is used to remove **(dequeue)** data called **front** . Queue follows First-In-First-Out methodology, i.e., the data item stored first will be accessed first.***


***Queue operations may involve initializing or defining the queue, utilizing it, and then completely erasing it from the memory. Here we shall try to understand the basic operations associated with queues beside enqueue and dequeue :***


- **peek()** : *Gets the element at the front of the queue without removing it.*

- **isfull()** : *Checks if the queue is full.*

- **isempty()** : *Checks if the queue is empty.*



![IMG](https://4cawmi2va33i3w6dek1d7y1m-wpengine.netdna-ssl.com/wp-content/uploads/2018/07/Computer-science-fundamentals_6.1.png)

