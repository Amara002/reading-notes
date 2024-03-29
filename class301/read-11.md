# What is OAuth


1. **What is OAuth?**
***OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.***

2. **Give an example of what using OAuth would look like.**
***when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logo***

3. **How does OAuth work? What are the steps that it takes to authenticate the user?**
***Let’s assume a user has already signed into one website or service, The following happens***

- ***The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.***
- ***The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.***
- ***The first site gives this token and secret to the initiating user’s client software.***
- ***The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).***
- ***If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.***
- ***The user approves (or their software silently approves) a particular transaction type at the first website.***
- ***The user is given an approved access token (notice it’s no longer a request token).***
- ***The user gives the approved access token to the first website.***
- ***The first website gives the access token to the second website as proof of authentication on behalf of the user.***
- ***The second website lets the first website access their site on behalf of the user.***
- ***The user sees a successfully completed transaction occurring.***
- ***OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).***

4. **What is OpenID?**
***It is a security technology and it is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.***


# Authorization and Authentication flows

1. **What is the difference between authorization and authentication?**
***Auth0 uses the OpenID Connect (OIDC) Protocol and OAuth 2.0 Authorization Framework to authenticate users and get their authorization to access protected resources. With Auth0, you can easily support different flows in your own applications and APIs without worrying about OIDC/OAuth 2.0 specifications or other technical aspects of authentication and authorization.***

2. **What is Authorization Code Flow?**
***Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token***

3. **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**
***During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).***

4. **What is Implicit Flow with Form Post?**
***pplications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.***

5. **What is Client Credentials Flow?**
***With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don’t make sense. Instead, M2M apps use the Client Credentials Flow***

6. **What is Device Authorization Flow?**
***is an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. This is commonly seen on Apple TV apps, or devices like hardware encoders that can stream video to a YouTube channel.***
