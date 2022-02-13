# OAuth 2.0 - Basic Understanding

This write is about:

+ What OAuth is
+ OAuth terminology
+ Authorization and scope
+ The work flow of OAuth

## What is OAuth ?

OAuth stand for `Open Authentication` or `Open Authorization`. As the name, it is invented to solve authentication and authorization for sharing data to various application without create new account or share **username** and **password**

`Authentication`: is the to prove that the user exist and correct

`Authorization`:  is the permission for the application to access the data (user will authorize the app to access their data)

So, if you see some app that allow you to enter using your Facebook or Google account, that is form of OAuth.



## OAuth 2.0 Terminology

+ Resource owner : who own the data that application wants to access to

- Client: is the application that wants to access the data

- Authorization server: the server to authorize data access for application

- Resource server: where application access to read the data

- Authorization grant: is the process to prove that user is actually allow the application to access data

- Redirect URI (callback) : is where to redirect after the user authorization granted

- Access token: is the key to prove to the resource server that the application has authorized to access data

  

## How OAuth work ?

1. Application will make an authorization request to user. (with callback and scope)
2. User will be redirected to an authorization server.
3. After user is authenticated on, for example, Google server and authorized the application, they will be redirected to a callback URI with an `authorization code`.
4. Application then, exchange the authorization code into an access token within the given scope.
5. Application will request for the data at `Resource server` with an `access token`

