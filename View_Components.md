# View Components 

## What is View Components ?

***As part of ASP.NET MVC 6, a new feature called view components has been introduced. View components are similar to child actions and partials views, allowing you to create reusable components with (or without) logic .***

***A view component consists of two parts, the class (typically derived from ViewComponent ) and the result it returns (typically a view). Like controllers, a view component can be a POCO ( plain old class object ), but most developers will want to take advantage of the methods and properties available by deriving from ViewComponent .***

![IMG](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/viewcomponent-in-asp-net-core/Images/ViewComponent5.png)

## View Components specifications :

- **Renders a chunk rather than a whole response.**

- **Includes the same separation-of-concerns and testability benefits found between a controller and view.**

- **Can have parameters and business logic.**

- **Is typically invoked from a layout page.**


## The view component class

***A view component class can be created by any of the following:***

- **Deriving from ViewComponent**

- **Decorating a class with the ViewComponent attribute, or deriving from a class with the ViewComponent attribute**

- **Creating a class where the name ends with the suffix ViewComponent**

***A view component class:***

- **Supports constructor dependency injection**

- **Doesn't take part in the controller lifecycle, therefore filters can't be used in a view component**


## View component methods

***A view component defines its logic in an:***

- **```InvokeAsync``` method that returns ```Task<IViewComponentResult>```.**

- **```Invoke``` synchronous method that returns an IViewComponentResult.**


# Summary

***ASP.NET MVC 6 introduces view components, a component-oriented mixture of child actions and partial views. They can return various content, including Razor views, JSON, or plain text. View components can be rendered synchronously or asynchronously. Finally, they can integrate with the dependency injection system of ASP.NET Core through constructor injection.***
