# Cookies

## What are Cookies ?

***Cookies are text files with small pieces of data — like a username and password — that are used to identify your computer as you use a computer network. Specific cookies known as **HTTP cookies** are used to identify specific users and improve your web browsing experience.***

***Data stored in a cookie is created by the server upon your connection. This data is labeled with an ID unique to you and your computer.***

***When the cookie is exchanged between your computer and the network server, the server reads the ID and knows what information to specifically serve to you.***

## Cookies Usings :

***Cookies mainly used for three purposes:***

- **Session management**

***Logins, shopping carts, game scores, or anything else the server should remember***

- **Personalization**

***User preferences, themes, and other settings***

- **Tracking**

***Recording and analyzing user behavior***

![IMG](https://www.georanker.com/app/uploads/2014/09/cookie.jpg)

## Creating cookies :

***After receiving an HTTP request, a server can send one or more Set-Cookie headers with the response. The browser usually stores the cookie and sends it with requests made to the same server inside a Cookie HTTP header. You can specify an expiration date or time period after which the cookie shouldn't be sent. You can also set additional restrictions to a specific domain and path to limit where the cookie is sent.***

### The ```Set-Cookie``` and ```Cookie``` headers :

***The ```Set-Cookie``` HTTP response header sends cookies from the server to the user agent. A simple cookie is set like this:***

```
Set-Cookie: <cookie-name>=<cookie-value>
```

***This instructs the server sending headers to tell the client to store a pair of cookies:***

```
HTTP/2.0 200 OK
Content-Type: text/html
Set-Cookie: yummy_cookie=choco
Set-Cookie: tasty_cookie=strawberry

[page content]
```

***Then, with every subsequent request to the server, the browser sends all previously stored cookies back to the server using the ```Cookie``` header.***

```
GET /sample_page.html HTTP/2.0
Host: www.example.org
Cookie: yummy_cookie=choco; tasty_cookie=strawberry
```


## Different types of cookies

- **Magic Cookies** : ***are an old computing term that refers to packets of information that are sent and received without changes. Commonly, this would be used for a login to computer database systems, such as a business internal network. This concept predates the modern “cookie” we use today.***

- **HTTP Cookies**


# HTTP Cookies

***HTTP cookies are a repurposed version of the “magic cookie” built for internet browsing. Web browser programmer Lou Montulli used the “magic cookie” as inspiration in 1994. He recreated this concept for browsers when he helped an online shopping store fix their overloaded servers.***

***HTTP cookie (web cookie, browser cookie) is a small piece of data that a server sends to a user's web browser. The browser may store the cookie and send it back to the same server with later requests. Typically, an HTTP cookie is used to tell if two requests come from the same browser—keeping a user logged in, for example. It remembers stateful information for the stateless HTTP protocol.***

***The HTTP cookie is what we currently use to manage our online experiences. It is also what some malicious people can use to spy on your online activity and steal your personal info.***


***HTTP cookies are essential to the modern Internet but a vulnerability to your privacy. As a necessary part of web browsing, HTTP cookies help web developers give you more personal, convenient website visits. Cookies let websites remember you, your website logins, shopping carts and more.***

