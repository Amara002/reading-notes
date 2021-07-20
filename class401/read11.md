# Spring

## Serving Web Content with Spring MVC

**Manual Initialization**

***If you want to initialize the project manually rather than use the links shown earlier, follow the steps given below:***
1. ***Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.***

2. ***Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.***

3. ***Click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools.***

4. ***Click Generate.***

5. ***Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.***

> ***If your IDE has the Spring Initializr integration, you can complete this process from your IDE.***

## Spring MVC and Thymeleaf: how to access data from templates

1. ***Spring model attributes: Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.***

2. ***Request parameters: Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server like:***<br>
***https://example.com/query?q=Thymeleaf+Is+Great!***

3. ***Session attributes: milarly to the request parameters, session attributes can be accessed by using the session. prefix***

4. ***ServletContext attributes: The ServletContext attributes are shared between requests and sessions. In order to access ServletContext attributes in Thymeleaf you can use the #servletContext. prefix***

5. ***Spring beans: Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax.***


