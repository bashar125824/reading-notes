# Introduction to Identity on ASP.NET Core

***ASP.NET Core Identity is an API that supports user interface (UI) login functionality , Manages users, passwords, profile data, roles, claims, tokens, email confirmation, and more.***

![IMG](https://fullstackmark.com/img/posts/21/oauth-openid-connect-architecture-angular-spa-aspnet-core-mvc-web-api-identityserver4.png)


***Users can create an account with the login information stored in Identity or they can use an external login provider. Supported external login providers include Facebook, Google, Microsoft Account, and Twitter.***

***ASP.NET Core Identity adds user interface (UI) login functionality to ASP.NET Core web apps. To secure web APIs and SPAs, use one of the following*** :

- **Azure Active Directory**
- **Azure Active Directory B2C (Azure AD B2C)**
- **IdentityServer4**

## What is IdentityServer4 ?

***It's an OpenID Connect and OAuth 2.0 framework for ASP.NET Core. IdentityServer4 enables the following security features*** :

- **Authentication as a Service (AaaS)**
- **Single sign-on/off (SSO) over multiple application types**
- **Access control for APIs**
- **Federation Gateway**

---

# ASP.NET Core 2.0 Authentication and Authorization System 

**Authentication** : *is the process of determining a user's identity* 
**Authorization** :  *is the process of determining whether a user has access to a resource*

***In ASP.NET Core, authentication is handled by the authentication service, IAuthenticationService, which is used by authentication middleware . The authentication service uses registered authentication handlers to complete authentication-related actions. Examples of authentication-related actions include*** :

- **Authenticating a user**
- **Responding when an unauthenticated user tries to access a restricted resource**

## Some principles to know :

- **Claims** : *A Claim represents a single fact about the user. It could be the user's first name, last name, age, employer, birth date, or anything else that is true about the user. A single claim will contain only a single piece of information. A claim representing something about a user John Smith could be his first name: John. A second claim would be his last name: Smith.*

*Claims are represented by the Claim class in ASP.Net Core. It's most common constructor accepts two strings: type and value. The 'type' parameter is the name of the claim, while the value is the information the claim is representing about the user.*

- **Verbs** : *There are 5 verbs (these can also be thought of as commands or behaviors) that are invoked by the auth system, and are not necessarily called in order. These are all independent actions that do not communicate among themselves, however, when used together allow users to sign in and access pages otherwise denied. Here is a very brief description of what each verb is responsible for*

***the 5 verbs :***

1. **Authenticate**
*Gets the user’s information if any exists (e.g. decoding the user’s cookie, if one exists)*

2. **Challenge**
*Requests authentication by the user (e.g. showing a login page)*

3. **SignIn**
*Persists the user’s information somewhere (e.g. writes a cookies)*

4. **SignOut**
*Removes the user’s persisted information (e.g. deletes the cookies)*

5. **Forbid**
*Denies access to a resource for unauthenticated users or authenticated but unauthorized users (e.g. displaying a “not authorized” page)*

