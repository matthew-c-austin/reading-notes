# Read: Class 32

## Reflections

This reading assignment talks about Serverless, more info about Amplify, and an impenetrable and opaque bit of documentation about GraphQL

## Readings

[Intro to Serverless](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

[AWS Amplify](https://aws.amazon.com/amplify/)

[GraphQL Intro](https://docs.amplify.aws/cli/graphql/data-modeling/)

1. What makes an API RESTful?

    A RESTful API (Representational State Transfer) adheres to a set of constraints or architectural styles for building web services. The key characteristics include:

    - Stateless: Each client request must contain all the information necessary to process the request. The server must not store anything about the latest HTTP request the client made.

    - Client-Server: The client and the server are two separate entities that communicate over HTTP, and they can evolve separately without any dependency on each other.

    - Cacheable: Responses from the server can be cached by the client in order to improve performance.

    - Uniform Interface: A RESTful API should have a predictable, standardized interface, making it easier for clients to understand how to interact with it.

    - Layered System: The architecture can be composed of multiple layers, each with specific functionality. This improves scalability and flexibility.

2. What is the benefit of using GraphQL? Any downsides?

    GraphQL is a query language for APIs that enables clients to request exactly what data they need, and nothing more. It has several benefits:

    - Precise Data Fetching: This means less over-fetching or under-fetching of data compared to REST, which can improve performance and efficiency.

    - Single Request-Response: Instead of making multiple requests to different endpoints (like in REST), GraphQL can fetch all required data in a single request.

    - Strong Typing: GraphQL schemas are strongly typed. This leads to clear contracts, making it easier to reason about the data and catch errors earlier.

    However, there are also downsides:

    - Complexity: GraphQL can be overkill for simple APIs and adds complexity to the development process.

    - Learning Curve: It can take some time for developers to understand and use GraphQL effectively.

    - Caching: While GraphQL allows precise queries, this can make client-side caching more complex compared to REST, which can simply cache URLs.

3. Describe “serverless” to a new 301 Code Fellows student.

    "Serverless" is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral, and fully managed by the cloud provider.

    In other words, the term "serverless" means developers don't need to worry about server management tasks like scaling, patching, capacity planning, etc. Instead, they can focus solely on writing code for their application, while the underlying infrastructure is handled by the cloud provider.

    Keep in mind though, "serverless" doesn't mean there are no servers involved; it just means the developers don't need to manage them.

## Things I want to know more about

1. Just thinking about what it would take to deploy our midterm on AWS, and I'm getting the notion that it would take a lot of work to modify it.
