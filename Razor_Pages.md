# Razor Pages

## What is Razor Pages ?

***Razor Pages is a newer, simplified web application programming model. It removes much of the ceremony of ASP.NET MVC by adopting a file-based routing approach. Each Razor Pages file found under the Pages directory equates to an endpoint.***

***Razor Pages have an associated C# objected called the page model, which holds each page's behavior. Additionally, each page works on the limited semantics of HTML, only supporting ```GET``` and ```POST``` methods.***

***Razor Pages can make coding page-focused scenarios easier and more productive than using controllers and views.***


![IMG](https://docs.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/razor-pages-start/_static/home2.2.png?view=aspnetcore-6.0)


## Why Razor Pages ?

***MVC developers want probably ask why we need one more way to build web sites on ASP.NET Core? Isn’t MVC enough? From information I have found from public space I found the following reasoning :***

- **It’s easier to get to web development for beginners as Razor pages are more lightweight than MVC. Besides beginners there are people who are coming from other scripting languages be it old ASP or PHP or something else.**

- **Razor Pages fit well to smaller scenarios where building controllers and models as separate classes is overkill.**

## MVC vs RAZOR PAGES

***A Razor Page is almost the same as ASP.NET MVC’s view component. It has basically the syntax and functionality same as MVC.***

***The basic difference between Razor pages and MVC is that the model and controller code is also added within the Razor Page itself. You do not need to add code separately.***

***It is similar to MVVM (Model-View-View-Model) framework. That provides two-way data binding and a simpler development experience with isolated concerns.***

***The ASP.NET MVC has been extremely popular nowadays for web application development, and it definitely has lots of advantages. In fact, the ASP.NET Web Forms was particularly designed as an MVVM solution in MVC.***

***But, the new ASP.NET Core Razor Pages is the next development of ASP.NET Web Forms***
 
## Basic Structure of Razor Pages and MVC

***Razor pages do not have any type of structure like MVC. But all Razor pages inbuilt under the Pages folder with a very simple structure. You have to see the below screenshot for more understanding. Further, you can organize your project structure based on your requirements.***


![IMG](https://ifourtechnolab.ifour-consultancy.net/Uploads/Post/razor1.webp)

![IMG](https://ifourtechnolab.ifour-consultancy.net/Uploads/Post/razor2.webp)


## Create Razor Pages 

***Razor Pages is enabled in ```Program.cs```:***

```
var builder = WebApplication.CreateBuilder(args);

builder.Services.AddRazorPages();

var app = builder.Build();

if (!app.Environment.IsDevelopment())
{
    app.UseExceptionHandler("/Error");
    app.UseHsts();
}

app.UseHttpsRedirection();
app.UseStaticFiles();

app.UseRouting();

app.UseAuthorization();

app.MapRazorPages();

app.Run();

```

***Basic Page :***

```
@page

<h1>Hello, world!</h1>
<h2>The time on the server is @DateTime.Now</h2>

```