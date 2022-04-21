# Routing in ASP.NET Core

***Routing is responsible for matching incoming HTTP requests and dispatching those requests to the app's executable endpoints. Endpoints are the app's units of executable request-handling code. Endpoints are defined in the app and configured when the app starts. The endpoint matching process can extract values from the request's URL and provide those values for request processing. Using endpoint information from the app, routing is also able to generate URLs that map to endpoints.***

**Apps can configure routing using :**

- *Controllers*
- *Razor Pages*
- *SignalR*
- *gRPC Services*
- *Endpoint-enabled middleware such as Health Checks*
- *Delegates and lambdas registered with routing.*


# What is ASP.NET MVC Routing ?

***ASP.NET MVC routing is a pattern matching system that is responsible for mapping incoming browser requests to specified MVC controller actions***

![IMG](https://csharpcorner-mindcrackerinc.netdna-ssl.com/UploadFile/3d39b4/routing-in-mvc/Images/ASP.NET%20MVC%20Routing.jpg)

## Default Route Table

***When you create a new ASP.NET MVC application, the application is already configured to use ASP.NET Routing. ASP.NET Routing is setup in two places.***

***First, ASP.NET Routing is enabled in your application's Web configuration file (Web.config file). There are four sections in the configuration file that are relevant to routing: the system.web.httpModules section, the system.web.httpHandlers section, the system.webserver.modules section, and the system.webserver.handlers section. Be careful not to delete these sections because without these sections routing will no longer work.***

***Second, and more importantly, a route table is created in the application's Global.asax file. The Global.asax file is a special file that contains event handlers for ASP.NET application lifecycle events. The route table is created during the Application Start event.***

