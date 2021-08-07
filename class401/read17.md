# Spring Boot and OAuth2



***There are several samples building on each other, adding new features at each step:***

- **simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).**

- **click: adds an explicit link that the user has to click to login.**

- **logout: adds a logout link as well for authenticated users.**

- **two-providers: adds a second login provider so the user can choose on the home page which one to use.**

- **custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.**

## How to Add a Local User Database

***Many applications need to hold data about their users locally, even if authentication is delegated to an external provider. We don’t show the code here, but it is easy to do in two steps.***

- **Choose a backend for your database, and set up some repositories (using Spring Data, say) for a custom User object that suits your needs and can be populated, fully or partially, from external authentication.**

- **Implement and expose OAuth2UserService to call the Authorization Server as well as your database. Your implementation can delegate to the default implementation, which will do the heavy lifting of calling the Authorization Server. Your implementation should return something that extends your custom User object and implements OAuth2User.**

## Notes

***We have seen how to use Spring Boot and Spring Security to build apps in a number of styles with very little effort. The main theme running through all of the samples is authentication using an external OAuth 2.0 provider.***

***All of the sample apps can be easily extended and re-configured for more specific use cases, usually with nothing more than a configuration file change. Remember if you use versions of the samples in your own servers to register with GitHub (or similar) and get client credentials for your own host addresses. And remember not to put those credentials in source control!***
