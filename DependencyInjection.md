# What is Dependency Injection ?

***Dependency Injection (DI) is a design pattern used to implement IoC. It allows the creation of dependent objects outside of a class and provides those objects to a class through different ways. Using DI, we move the creation and binding of the dependent objects outside of the class that depends on them***

***Inversion of Control(IoC) is also known as Dependency injection (DI).***

***technique for achieving Inversion of Control (IoC) between classes and their dependencies.***

***The Dependency Injection pattern involves 3 types of classes :***

- **Client Class** : *The client class (dependent class) is a class which depends on the service class*

- **Service Class** : *The service class (dependency) is a class that provides service to the client class*

**Injector Class** : *The injector class injects the service class object into the client class*

![IMG](https://www.tutorialsteacher.com/Content/images/ioc/DI.png)


***A dependency is an object that another object depends on. Examine the following ```MyDependency``` class with a ```WriteMessage``` method that other classes depend on:***

```

public class MyDependency
{
    public void WriteMessage(string message)
    {
        Console.WriteLine($"MyDependency.WriteMessage called. Message: {message}");
    }
}

```

---

# The Repository pattern

***Repositories are classes or components that encapsulate the logic required to access data sources. They centralize common data access functionality, providing better maintainability and decoupling the infrastructure or technology used to access databases from the domain model layer. If you use an Object-Relational Mapper (ORM) like Entity Framework, the code that must be implemented is simplified, thanks to LINQ and strong typing. This lets you focus on the data persistence logic rather than on data access plumbing.***


## Define one repository per aggregate :

***For each aggregate or aggregate root, you should create one repository class. In a microservice based on Domain-Driven Design (DDD) patterns, the only channel you should use to update the database should be the repositories. This is because they have a one-to-one relationship with the aggregate root, which controls the aggregate's invariants and transactional consistency. It's okay to query the database through other channels (as you can do following a CQRS approach), because queries don't change the state of the database. However, the transactional area (that is, the updates) must always be controlled by the repositories and the aggregate roots.***

![IMG](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/media/infrastructure-persistence-layer-design/repository-aggregate-database-table-relationships.png)

## Enforce one aggregate root per repository :

***It can be valuable to implement your repository design in such a way that it enforces the rule that only aggregate roots should have repositories. You can create a generic or base repository type that constrains the type of entities it works with to ensure they have the ```IAggregateRoot``` marker interface :***

```

namespace Microsoft.eShopOnContainers.Services.Ordering.Infrastructure.Repositories
{
    public class OrderRepository : IOrderRepository
    {
      // ...
    }
}

```

---

# SOLID principals :

***The SOLID Principals of software development is the brain child or Robert “Uncle Bob” Martin. In the early 2000 he described five principals that software developers could use to guide them in creating software that was well designed, high quality and easier to maintain than what was being produced at the time. These five ideas are simple, promote good practices in software design and development, and go a long way to help us in our practice of TDD.***

1. **Single Responsibility Principle** : ***The Single Responsibility Principal (SRP) is the idea that every method or class in your application should have exactly one reason to change. You can logically extend that to say that every class or method in your application should have exactly one (a single) job or responsibility. The short way of saying this is that each method and each class should be responsible for one, and only one task***

2. **The Open/Close Principle** :  ***The Open/Close Principle (OCP) is very closely related to the previously discussed topics of Encapsulation and Inheritance. In fact it’s fair to say the OCP is concept that unifies these two tenants of OOP. OCP states that software, be it a method or a class, should be open for extension, but closed to modification***

3. **The Liskov Substitution Principle** : ***The Liskov Substitution Principle (LSP) states that an object in your application should be able to be replaced with a type derived from it without breaking the application***

4. **The Interface Segregation Principle** : ***The Interface Segregation Principle states that clients should not be forced to rely on interfaces they do not use. Another way to say this is that you should make fine grained interfaces that are specific to the functions and needs of the client***

5. **The Dependency Inversion Principle** : ***Coupling and binding in software is a fact of life. For all or our efforts to eliminate the need for binding, at the end of the day our classes have to bind to something to be usable***

---

# Why SOLID matters ?

***One of the biggest struggles that developers have with adopting Unit Testing, whether it’s Test Driven Development (TDD), Behavior Driven Development (BDD) or even just Test Eventual Development (TED), is the difficulty some code is to test.  This is typically when code doesn’t follow the SOLID design principles***

---

# SOLID principals in pictures :

1. ***S — Single Responsibility***

*A class should have a single responsibility*

![IMG](https://miro.medium.com/max/1400/1*P3oONz9Da3Tc1w97fMV73Q.png)

**Goal**

*This principle aims to separate behaviours so that if bugs arise as a result of your change, it won’t affect other unrelated behaviours*

2. ***O — Open-Closed***

*Classes should be open for extension, but closed for modification*

![IMG](https://miro.medium.com/max/1400/1*0MtFBmm6L2WVM04qCJOZPQ.png)

**Goal**

*This principle aims to extend a Class’s behaviour without changing the existing behaviour of that Class. This is to avoid causing bugs wherever the Class is being used.*

3. ***L — Liskov Substitution***

*If S is a subtype of T, then objects of type T in a program may be replaced with objects of type S without altering any of the desirable properties of that program.*

![IMG](https://miro.medium.com/max/1400/1*yKk2XKJaCLNlDxQMx1r55Q.png)

**Goal**

*This principle aims to enforce consistency so that the parent Class or its child Class can be used in the same way without any errors*

4. ***I — Interface Segregation***

*Clients should not be forced to depend on methods that they do not use*

![IMG](https://miro.medium.com/max/1400/1*2hmyR9L43Vm64MYxj4Y89w.png)

**Goal**

*This principle aims at splitting a set of actions into smaller sets so that a Class executes ONLY the set of actions it requires.*

5. ***D — Dependency Inversion***

- *High-level modules should not depend on low-level modules. Both should depend on the abstraction*

- *Abstractions should not depend on details. Details should depend on abstractions*

![IMG](https://miro.medium.com/max/1400/1*Qk8tDmjQlyvwKxNTfXIo0Q.png)

**Goal**

*This principle aims at reducing the dependency of a high-level Class on the low-level Class by introducing an interface*

