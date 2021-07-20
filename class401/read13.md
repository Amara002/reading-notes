# Related Resources and Integration Testing

## Working with Relationships in Spring Data REST

- **One-to-One Relationship**<br>
***define two entity classes Library and Address having a one-to-one relationship, using the @OneToOne annotation.***

- **One-to-Many Relationship**<br>
***A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.***

- **Many-to-Many Relationship**<br>
***A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.***

## Integration Testing in Spring

- **Preparation**
***Several Maven dependencies are required for running the integration tests. we'll need the latest junit-jupiter-engine, junit-jupiter-api, and Spring test dependencies***

- **Spring MVC Test Configuration**

1. ***Enable Spring in Tests with JUnit 5***<br>
***We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.***
2. ***The WebApplicationContext Object***<br>
***WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.***
3. ***Mocking Web Context Beans***<br>
***MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.***
4. ***Verify Test Configuration***<br>
***we're also checking that a GreetController.java bean exists in the web context. This ensures that Spring beans are loaded properly. At this point, the setup of the integration test is done.***


- **Writing Integration Tests**

1. ***Verify View Name***
2. ***Verify Response Body***
3. ***Send GET Request With Path Variable***
4. ***Send GET Request With Query Parameters***
5. ***Send POST Request***


