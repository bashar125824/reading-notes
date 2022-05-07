# Intro to claims :

## What is Claim ?

***A claim is a name value pair that represents what the subject is, not what the subject can do , claims can be created from any user or identity data which can be issued using a trusted identity provider or ASP.NET Core identity***

![IMG](https://andrewlock.net/content/images/2016/08/Untitled.png)

## The difference between Authentication and Authorisation : 

***First of all, we should clarify the difference between these two dependent facets of security. The simple answer is that Authentication is the process of determining who you are, while Authorisation revolves around what you are allowed to do, i.e. permissions. Obviously before you can determine what a user is allowed to do, you need to know who they are, so when authorisation is required, you must also first authenticate the user in some way***

# Claims-based authorization in ASP.NET Core : 

## Claim based authorization checks :

- **Are declarative**
- **Are applied to Razor Pages, controllers, or actions within a controller**
- **Can not be applied at the Razor Page handler level, they must be applied to the Page**

# JWT to authenticate Servers API’s :

## What is JWT ?

***JSON Web Token (JWT) is a means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS) and/or encrypted using JSON Web Encryption (JWE)***

***In simple terms, it is just another way of encoding JSON object and use that encoded object as access tokens for authentication from the server.***

## the practical application of JWT :

- **JWT for downloading the files at the client**
- **JWT for the server to server authentication**