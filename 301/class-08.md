# Reading

[API Design Best Practices](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. What does REST stand for?

    Representational State Transfer

2. REST APIs are designed around a ____.

    Resource

3. What is an identifier of a resource? Give an example.

    A URI (Uniform Resource Identifier) that uniquely identifies it.

4. What are the most common HTTP verbs?

    The most common operations are GET, POST, PUT, PATCH, and DELETE.

5. What should the URIs be based on?

    Nouns (the resource) and not verbs (the operations on the resource)

6. Give an example of a good URI.

    `https://adventure-works.com/orders`

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    All web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.

8. What status code does a successful GET request return?

    200 (OK)

9. What status code does an unsuccessful GET request return?

    Depends. 404 for no found resource, 204 if teh body included in the response is empty.

10. What status code does a successful POST request return?

    201 (Created)

11. What status code does a successful DELETE request return?

    204 (No Content)

## Things I want to know more about

1. There's so much to know here it's almost like asking what more you want to know about programming. Creating APIs is an entire career.
