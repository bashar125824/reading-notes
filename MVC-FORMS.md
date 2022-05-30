# Views in ASP.NET Core MVC :

## What is View in MVC ?

***A View, in the context of a Model View Controller (MVC) architecture, is a software class that contains a template and data form and produces a response for the browser. It receives data from the Controller of the MVC and packages it and presents it to the browser for display.***

***The View is not very autonomous -it is like a black box where some data is thrown at it and it gives a display to the user in a browser friendly manner. It collects the input data from data sources, finds the template upon invocation, and combines them into HTML output at runtime.***

***In ASP.NET Core MVC, views are ```.cshtml``` files that use the C# programming language in Razor markup. Usually, view files are grouped into folders named for each of the app's controllers.***

## Benefits of using views :


***Views help to establish separation of concerns within an MVC app by separating the user interface markup from other parts of the app. Following SoC design makes your app modular, which provides several benefits:***

- **The app is easier to maintain because it's better organized. Views are generally grouped by app feature. This makes it easier to find related views when working on a feature.**

- **The parts of the app are loosely coupled. You can build and update the app's views separately from the business logic and data access components. You can modify the views of the app without necessarily having to update other parts of the app.**

- **It's easier to test the user interface parts of the app because the views are separate units.**

- **Due to better organization, it's less likely that you'll accidentally repeat sections of the user interface.**

## Pass data to views :

***Pass data to views using several approaches:***

- **Strongly typed data : viewmodel**

- **Weakly typed data :**

1. **ViewData (ViewDataAttribute)**
2. **ViewBag**

---

# MVC Forms

***MVC forms are part of ASP.NET MVC framework , MVC technology provides a modern, convention-based, mobile-first UI framework to quick and easy setup and design of forms and applications. Thanks to the MVC pattern, you can separate development into views, logic, and processing , Forms are very essential and basic thing that every programmer has to learn .***

![IMG](https://i.stack.imgur.com/FBrcZ.png)

## 4 Different Ways to Create ASP.NET MVC Forms :

1. **Forms - Weakly Typed (Synchronous)**
2. **Forms - Strongly Typed (Synchronous)**
3. **Forms - Strongly Typed AJAX (Asynchronous)**
4. **Forms – HTML, AJAX and JQUERY**

### 1- FORMS – WEAKLY TYPED :

***his is the easiest and quickest way to create forms in MVC.***

***Advantage :***

1. *It is easy to create a form using Weakly Typed mechanism*
2. *Mostly used when you need to create a form with one or two input items.*

***Disadvantage:***

1. *Because, it is not strongly typed so IntelliSense doesn't help you.*
2. *Have higher chance of getting exception and runtime error messages.*
3. *Very difficult to manage when forms have multiple input items and controls.*
4. *It is very clumsy when you need to add or remove some input items.*

### 2- FORMS – WEAKLY TYPED :

***In this method, we send objects (model) instead of sending each item as parameter. It is easy to maintain because you don't need to remember each input item and IntelliSense will show you automatically the each item.***

### 3- FORMS - STRONGLY TYPED AJAX (ASYNCHRONOUS)

***Asynchronous AJAX form is a very magical way to submit data to the controller without happening page load. Asynchronous AJAX Forms simply post back the data to the controllers and update the only that part of the page, which has to display output.***

***To make this happen, we will use JQuery-Unobstrusive-AJAX. This is a great feature which is launched in MVC 3. It helps you to create AJAX Form without writing bunch of javascript code. Before creating Asynchronous AJAX Form you need to add JQuery-Unobstrusive-AJAX in your project. Adding is very easy, and just follows the steps.***

### 4. PURE HTML FORMS WITH AJAX AND JQUERY

***In this method, you can not only send data from input controls but can also use html elements like <p>…</p>, <span>…</span> to send data to controllers. This is pure JQuery and AJAX query.***
