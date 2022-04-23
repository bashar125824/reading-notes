# What is DTO's ?

***A Data Transfer Object (commonly known as a DTO) is usually an instance of a POCO (plain old CLR object) class used as a container to encapsulate data and pass it from one layer of the application to another. You would typically find DTOs being used in the service layer to return data back to the presentation layer. The biggest advantage of using DTOs is decoupling clients from your internal data structures.***

***DTO is only used to pass data and does not contain any business logic. They only have simple setters and getters.***

![IMG](https://docs.microsoft.com/en-us/archive/msdn-magazine/2009/august/images/ee236638.fig01_l(en-us,msdn.10).gif)

***For example, below is an Entity class or a business class. You can see that it has business logic in the setters :***

```
class CustomerBO
{
        private string _CustomerName;
        public string CustomerName
        {
            get { return _CustomerName; }
            set 
            {
                if (value.Length == 0)
                {
                    throw new Exception("Customer name is required");
                }
                _CustomerName = value; 
            }
        }
}

```

***A data transfer object of the above Customer entity class would look something as shown below. It will only have setters and getters that means only data and no business logic.***

```

class CustomerDTO
{
        public string CustomerName { get; set; }
}

```

---

## Why use Data Transfer Objects (DTOs)?

***When designing and developing an application, if you’re using models to pass data between the layers and sending data back to the presentation layer, then you’re exposing the internal data structures of your application. That’s a major design flaw in your application.***

***By decoupling your layers DTOs make life easier when you’re implementing APIs, MVC applications, and also messaging patterns such as Message Broker. A DTO is a great choice when you would like to pass a lightweight object across the wire — especially when you’re passing your object via a medium that is bandwidth-constrained.***

---

## Use DTOs for abstraction

***You can take advantage of DTOs to abstract the domain objects of your application from the user interface or the presentation layer. In doing so, the presentation layer of your application is decoupled from the service layer. So if you would like to change the presentation layer, you can do that easily while the application will continue to work with the existing domain layer. Similarly, you can change the domain layer of your application without having to change the presentation layer of the application.***

---

## Use DTOs for data hiding

***Another reason you would want to use DTOs is data hiding. That is, by using DTOs you can return only the data requested. As an example, assume you have a method named GetAllEmployees() that returns all the data pertaining to all employees. Let’s illustrate this by writing some code.***