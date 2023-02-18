# Reading

[CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

1. Which HTTP method would you use to update a record through an API?

    PUT

2. Which REST methods require an ID parameter?

    Update/Delete

[Speed Coding: Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

1. What’s the relationship between REST and CRUD?

    While CRUD defines the basic operations that can be performed on data in a system, REST defines a set of principles for designing APIs that expose those operations as resources accessible through well-defined HTTP methods. In other words, RESTful APIs can implement CRUD operations, but they also provide additional constraints and principles for building scalable and maintainable systems.

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

    1. Define the resources: The first step in creating a RESTful API is to define the resources that will be exposed through the API.

    2. Choose the HTTP methods: The next step is to choose the HTTP methods that will be used to interact with each resource.

    3. Design the data model: Once the resources and HTTP methods have been defined, the next step is to design the data model that will be used to store the data associated with each resource.

    4. Implement the API endpoints: With the resources, HTTP methods, and data model defined, the next step is to implement the API endpoints.

    5. Document the API: The final step is to document the API so that other developers can understand how to use it.

## Things I want to know more about

1. I've noticed in both the videos that `express.Routes()` is used for all the HTTP methods. Is this the best practice vs. using an object with methods in it to export?
