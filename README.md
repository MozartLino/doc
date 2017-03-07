## Documentation ##

This document has as a main objective to explain how to integrate different domains, the Single Sign-on, which is defined as a single point of entry, you only need to authenticate once. This allows automatic access to multiple channels without the need to enter your login and password on each system, which provides more security to your authentication data.
We are using OAuth authorization framework enables a third-party application to obtain access.


## What is OAuth? ##

OAuth is an open protocol to allow secure authorization in a simple and standard method from web, mobile and desktop applications. As an application developer, services that provide HTTP APIs supporting OAuth, let you access parts of their service on behalf of your users. For example, when accessing a social network site, if your user gives you permission to access his account, you might be able to import pictures, friends lists, or contact information to your application. 

#### Some terms ####

Below contains definitions to fundamental protocol concepts referenced throughout the spec. Because understanding OAuth depends on these terms, they deserve some explanation:


* **Service Provider** – the Service Provider controls all aspects of the OAuth implementation. The Service Provider is the term used to describe the website or web-service where the restricted resources are located. It can be a photo sharing site where users keep albums, an online bank service, a microblogging site, or any other service where ‘user’s private stuff’ is kept. OAuth does not mandate that the Service Provider will also be the identity provider which means the Service Provider can use its own usernames and passwords to authenticate users, or use other systems such as OpenID.

* **User** – the user is why OAuth exists and without users, there is no need for OAuth. The users have ‘stuff’ they don’t want to make public on the Service Provider, but they do want to share it with another site. In OAuth, the protocol stops without manual interaction with the user at least once to receive permission to grant access.

* **Client** – this is a fancy name for an application trying to access the User’s resources. This can be a website, a desktop program, a mobile device, a set-top box, or anything else connected to the web. The Client is the one getting permission to access resources and the Client is where the useful part of OAuth happens. OAuth defines Client Developer’ as the entity writing code to interact with the Service Provider. 

* **Protected Resources** - the ‘stuff’ OAuth protects and allow access to. This can be data (photos, documents, contacts), activities (posting blog item, transferring funds) or any URL with a need for access restrictions.

* **Tokens** – are used instead of User credentials to access resources. A Token is generally a random string of letters and numbers (but not limited to) that is unique, hard to guess, and paired with a Secret to protect the Token from being abused. OAuth defines two different types of Tokens: Request and Access. This are explained later in greater details.





```
bundle exec rake sunspot:solr:reindex
```

`bundle exec bin/resque work -c ./.resque`
