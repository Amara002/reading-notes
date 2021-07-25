# Spring Security Architecture

***This guide is a primer for Spring Security, offering insight into the design and basic building blocks of the framework. We cover only the very basics of application security. However, in doing so, we can clear up some of the confusion experienced by developers who use Spring Security.***

## Authentication and Access Control
***Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?). Sometimes people say “access control” instead of "authorization", which can get confusing, but it can be helpful to think of it that way because “authorization” is overloaded in other places. Spring Security has an architecture that is designed to separate authentication from authorization and has strategies and extension points for both.***

## Customizing Authentication Managers
***Spring Security provides some configuration helpers to quickly get common authentication manager features set up in your application. The most commonly used helper is the `AuthenticationManagerBuilder`, which is great for setting up in-memory, JDBC, or LDAP user details or for adding a custom `UserDetailsService`.*** 


## Authorization or Access Control
***Once authentication is successful, we can move on to authorization, and the core strategy here is `AccessDecisionManager`. There are three implementations provided by the framework and all three delegate to a chain of `AccessDecisionVoter` instances, a bit like the `ProviderManager` delegates to `AuthenticationProviders`. An `AccessDecisionVoter` considers an `Authentication` (representing a principal) and a secure `Object`.***

## Web Security
***Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet `Filters`, so it is helpful to first look at the role of `Filters` generally. The following picture shows the typical layering of the handlers for a single HTTP request.***

## Method Security
***As well as support for securing web applications, Spring Security offers support for applying access rules to Java method executions. For Spring Security, this is just a different type of “protected resource”. For users, it means the access rules are declared using the same format of `ConfigAttribute` strings (for example, roles or expressions) but in a different place in your code.*** 