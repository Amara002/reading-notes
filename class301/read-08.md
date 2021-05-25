# API Design Best Practices


1. **What does REST stand for?**
***REST is an architectural style for building distributed systems based on hypermedia.***

2. **REST APIs are designed around a ____.**
***REST APIs are designed around resources.***

3. **What is an identifer of a resource? Give an example.**
***For example, the URI for a particular customer order might be:https://adventure-works.com/orders/1***

4. **What are the most common HTTP verbs?**
***The most common operations are GET, POST, PUT, PATCH, and DELETE.***

5. **What should the URIs be based on?**
***URIs should be based on nouns (the resource) and not verbs (the operations on the resource).***

6. **Give an example of a good URI.**
***It's a good practice to organize URIs for collections and items into a hierarchy. For example, /customers is the path to the customers collection, and /customers/5 is the path to the customer with ID equal to 5. This approach helps to keep the web API intuitive. Also, many web API frameworks can route requests based on parameterized URI paths, so you could define a route for the path /customers/{id}.***

7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**
***try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs. For more information about these performance antipatterns, see Chatty I/O and Extraneous Fetching.***

8. **What status code does a successful GET request return?**
***A successful GET method typically returns HTTP status code 200 (OK).***

9. **What status code does an unsuccessful GET request return?**
***If the resource cannot be found, the method should return 404 (Not Found).***

10. **What status code does a successful POST request return?**
***If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.***

11. **What status code does a successful DELETE request return?**
***If the delete operation is successful, the web server should respond with HTTP status code 204, indicating that the process has been successfully handled.***
