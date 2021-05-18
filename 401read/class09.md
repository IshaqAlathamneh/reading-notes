# Class 09

## What is OAuth?
OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password. This minimizes risk in a major way: In the event ESPN suffers a breach, your Facebook password remains safe.

OAuth doesn’t share password data but instead uses authorization tokens to prove an identity between consumers and service providers.

## How does OAuth work?

OAuth 2.0 was originally developed as a way of sharing access to specific data between applications. It works by defining a series of interactions between three distinct parties, namely a client application, a resource owner, and the OAuth service provider.

* Client application - The website or web application that wants to access the user's data.
* Resource owner - The user whose data the client application wants to access.
* OAuth service provider - The website or application that controls the user's data and access to it. They support OAuth by providing an API for interacting with both an authorization server and a resource server.

## Access Code

First the client needs to grant the application permission. To do this you need to provide an `<a>` tag that will take them to the service's authorization page. This `<a>` tag should pass the following information through a query string to the authorization server. Every service is slightly different in their specific requirements, but in some form or another, variables like these are part of this initial request.

- `response_type=code` indicates that your server wants to receive an authorization code
- `client_id=<your client id>` tells the authorization server which app the user is granting access to
- `redirect_uri=<your redirect uri>` tells the auth server which server endpoint to redirect to
- `scope=<list of scopes>` tells the auth server what you want the user to give access to
- `state=<anything you want>` a place where you can store info to pass to your server if you want


## OAuth Uses
Recognizing when an application is using OAuth authentication is relatively straightforward. If you see an option to log in using your account from a different website, this is a strong indication that OAuth is being used.

## Advantages of OAuth 2.0
It allows limited access to the user's data and allows accessing when authorization tokens expire. It has ability to share data for users without having to release personal information. It is easier to implement and provides stronger authentication.