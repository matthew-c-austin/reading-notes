# Read: Class 33

## Reflections

This reading assignment talks about how to establish one-to-many and many-to-one connections using GraphQL in AWS Amplify, and also explains the use of CompletableFuture in Java, which is a fundamental concept for handling asynchronous programming.

## Readings

[One-to-many and many-to-one connections using GraphQL in AWS Amplify](https://docs.amplify.aws/cli/graphql/data-modeling/#has-many-relationship)

[CompletableFuture in Java](https://www.baeldung.com/java-completablefuture)

1. Describe asynchronous actions in your own words.

    Essentially, it means that you can initiate a process and then carry on with other tasks without waiting for the initiated process to finish. Once the asynchronous operation is complete, it typically signals back by calling a callback function or resolving a promise.

2. What is the benefit of asynchronous methods?

    The benefit of asynchronous methods is they can significantly enhance the efficiency and performance of your program, particularly when dealing with IO operations (like network requests, file system tasks), where waiting for one operation to complete before starting another can lead to inefficient use of resources. By using asynchronous methods, your program can perform multiple operations concurrently without blocking or waiting, thereby improving overall throughput and responsiveness.

## Things I want to know more about

1. I feel like I barely touched the surface of asynchronous methods in Java in our midterm. Part of me wishes this was just a 100% Java focused course, and the back half would be associated with those types of topics.
