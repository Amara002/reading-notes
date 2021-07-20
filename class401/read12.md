# Spring RESTful Routing & Static Files

## Spring RequestMapping

- **@RequestMapping Basics**
1. ***@RequestMapping — by Path***
2. ***@RequestMapping — the HTTP Method***

-  **RequestMapping and HTTP Headers**
1. ***@RequestMapping With the headers Attribute***
2. ***@RequestMapping Consumes and Produces: Mapping media types produced by a controller method is worth special attention.We can map a request based on its Accept header via the @RequestMapping headers attribute***

- **RequestMapping With Path Variables**
1. ***Single @PathVariable***
2.  ***Multiple @PathVariable***
3. ***@PathVariable With Regex***

- **RequestMapping With Request Parameters**<br>
***@RequestMapping allows easy mapping of URL parameters with the @RequestParam annotation.***

- ***RequestMapping Corner Cases***
1. ***@RequestMapping — Multiple Paths Mapped to the Same Controller Method.***
***Although a single @RequestMapping path value is usually used for a single controller method (just good practice, not a hard and fast rule), there are some cases where mapping multiple requests to the same method may be necessary.***

2. ***@RequestMapping — Multiple HTTP Request Methods to the Same Controller Method.***
3. ***@RequestMapping — a Fallback for All Requests***
4. ***Ambiguous Mapping Error***<br>
***The ambiguous mapping error occurs when Spring evaluates two or more request mappings to be the same for different controller methods. A request mapping is the same when it has the same HTTP method, URL, parameters, headers, and media type.***

- **New Request Mapping Shortcuts**<br>
***Spring Framework 4.3 introduced a few new HTTP mapping annotations, all based on @RequestMapping:***

1. **@GetMapping**
2. **@PostMapping**
3. **@PutMapping**
4. **@DeleteMapping**
5. **@PatchMapping**

- **Spring Configuration**<br>
***The Spring MVC Configuration is simple enough, considering that our FooController.***

## CrudRepository, JpaRepository, and PagingAndSortingRepository in Spring Data

- **Spring Data Repositories**<br>
***Let's start with the JpaRepository – which extends PagingAndSortingRepository and, in turn, the CrudRepository.***

- **CrudRepository**<br>
***Notice the typical CRUD functionality:***
1. ***save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch***
2. ***findOne(…) – get a single entity based on passed primary key value***
3. ***findAll() – get an Iterable of all available entities in database***
4. ***count() – return the count of total entities in a table***
5. ***delete(…) – delete an entity based on the passed object***
6. ***exists(…) – verify if an entity exists based on the passed primary key value***

- **PagingAndSortingRepository**
***When using Pageable, we create a Pageable object with certain properties and we've to specify at least:***
1. ***Page size***
2. ***Current page number***
3. ***Sorting***

- **JpaRepository**
***Again, let's look at each of these methods in brief:***
1. ***findAll() – get a List of all available entities in database***
2. ***findAll(…) – get a List of all available entities and sort them using the provided condition***
3. ***save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch***
4. ***flush() – flush all pending task to the database***
5. ***saveAndFlush(…) – save the entity and flush changes immediately***
6. ***deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch***

- **Downsides of Spring Data Repositories**

    1. ***we couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; that's of course not unique to this library – but we do have to be careful not to expose these internal implementation details***
    2. ***by extending e.g. CrudRepository, we expose a complete set of persistence method at once. This is probably fine in most circumstances as well but we might run into situations where we'd like to gain more fine-grained control over the methods exposed, e.g. to create a ReadOnlyRepository that doesn't include the save(…) and delete(…) methods of CrudRepository***
