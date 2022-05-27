# Azure DevOps

## What is Azure DevOps?

***Azure DevOps developer services for allowing teams to plan work, collaborate on code development, and build and deploy applications. Azure DevOps supports a collaborative culture and set of processes that bring together developers, project managers, and contributors to develop software. It allows organizations to create and improve products at a faster pace than they can with traditional software development approaches.***

***Azure DevOps provides integrated features that you can access through your web browser or IDE client. You can use one or more of the following standalone services based on your business needs:***

- **Azure Repos** : *provides Git repositories or Team Foundation Version Control (TFVC) for source control of your code.*

- **Azure Pipelines** : *provides build and release services to support continuous integration and delivery of your applications.* 

- **Azure Boards** : *delivers a suite of Agile tools to support planning and tracking work, code defects, and issues using Kanban and Scrum methods.* 

- **Azure Test Plans** : *provides several tools to test your apps, including manual/exploratory testing and continuous testing.* 

- **Azure Artifacts** : *allows teams to share packages such as Maven, npm, NuGet, and more from public and private sources and integrate package sharing into your pipelines.* 


## Compare Azure DevOps Services with Azure DevOps Server :

***Azure DevOps Services are **cloud offering** , provides a scalable, reliable, and globally available hosted service. It's backed by a 99.9% SLA, monitored by our 24/7 operations team, and available in local data centers around the world.*** 

***Azure DevOps Server is **on-premises offering** , built on a SQL Server back end.***

## Fundamental differences between Azure DevOps Services and Azure DevOps Server :

***When you're choosing which platform you want, or if you're considering a move from on-premises to the cloud, consider the following areas:***

- **Scope and scale data**
- **Authentication**
- **Users and groups**
- **Manage user access**
- **Security and data protection**

---

# MVC Basics 

## What is MVC ?

***Model-View-Controller (MVC) is an architectural pattern that separates an application into three main logical components: the model, the view, and the controller. Each of these components are built to handle specific development aspects of an application. MVC is one of the most frequently used industry-standard web development framework to create scalable and extensible projects , it helps in developing the web application in a most efficient way when compared with the traditional ASP.NET Web Application.***

![IMG](https://www.tutorialspoint.com/mvc_framework/images/model_view_controller.jpg)

## differences between ASP.NET Web Application Framework and ASP.NET MVC Application Framework :

- **In traditional ASP.NET web application approach, the user action and view (UI) are combined, i.e., the web page, say, Sample.aspx and code behind Sample.aspx.cs which has the action logic are both tightly coupled, whereas in MVC, the View only deals with UI of the page and the user actions are defined in Controller.**

- **In any web based application, a user initiates the requests which are nothing but actions. So, for action based requirement, ASP.NET Web Application follows the View based architecture which is not so efficient. MVC is action-based architecture. Based on the action, an appropriate View is displayed. The organization of the code inside MVC is very clean and organized.**

- **In ASP.NET, View State is used to maintain the state of the web page. Maintaining the state means maintaining the data between post backs for a user. This makes the web page heavy which, in turn, makes the trips to server inefficient. In MVC, we don’t have View State to store the state information.**

- **ASP.NET MVC can be used to develop light-weight applications. This design pattern will also be useful when an application is being developed by large team as it can be controlled and maintained effectively. And one more advantage is that a few developers can work on View (UI part) and others on Models and others on Controller logic. And later, all the three can be integrated. It can also be used for large-scale applications.**

- **For RAD Models and small scale applications, it’s always better to go with traditional ASP.net Web Application Framework.**

---

# Tag Helpers

## What is Tag Helpers ?

***Tag Helpers enable server-side code to participate in creating and rendering HTML elements in Razor files .***

***For example, the built-in ```ImageTagHelper``` can append a version number to the image name. Whenever the image changes, the server generates a new unique version for the image, so clients are guaranteed to get the current image (instead of a stale cached image).***

## Example of Tag Helper :

***Consider a Razor view with the following model :***

```
public class Movie
{
    public int ID { get; set; }
    public string Title { get; set; }
    public DateTime ReleaseDate { get; set; }
    public string Genre { get; set; }
    public decimal Price { get; set; }
}
```

***The following Razor markup:***

```
<label asp-for="Movie.Title"></label>
```

***Generates the following HTML:***

```
<label for="Movie_Title">Title</label>
```

## Adavantage of Tag Helpers :

***Tag Helpers are attached to HTML elements inside your Razor views and can help you write markup that is both cleaner and easier to read than the traditional HTML Helpers. HTML Helpers, on the other hand, are invoked as methods that are mixed with HTML inside your Razor views***

---

# Bootstrap

## What is Bootstrap ?

***Bootstrap is potent front-end framework used to create modern websites and web apps. It's open-source and free to use, yet features numerous HTML and CSS templates for UI interface elements such as buttons and forms. Bootstrap also supports JavaScript extensions.***


