# Read: Class 13

## Reflections

This reading assignment talks about some data relationships in Spring, as well some integration testing methods for a web app using Spring and the MockMVC object.

## Readings

[Related data in Spring](https://www.baeldung.com/spring-data-rest-relationships)

1. Name a few real life examples of “One To Many” relatioships.

    - One bank account has many transactions.
    - One author writes many books.
    - One teacher has many students.

2. Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

   The Team is the "one" side, and the Player is the "many side.

3. Explain one to many relationships to a non-technical friend

   Imagine you're back in school. Each class has a teacher, and each teacher is responsible for many students. This is a one-to-many relationship.

[Baeldung: Spring Integration Testing](https://www.baeldung.com/integration-testing-in-spring)

1. Describe the difference between a unit test and an integration test.

    Unit tests focus on testing individual components in isolation, ensuring their functionality. Integration tests, on the other hand, test interactions between multiple components, validating their combined behavior. Unit tests are generally faster and use mocked dependencies, while integration tests are slower and involve real dependencies.

2. What is the object that provides support for Spring MVC Testing?

    `MockMvc` provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

    ```Java
    private MockMvc mockMvc;
    @BeforeEach
    public void setup() throws Exception {
        this.mockMvc = MockMvcBuilders.webAppContextSetup(this.webApplicationContext).build();
    }
    ```

3. What does the “perform()” method do in a Spring integration test?

    The `perform()` method will call a GET request method, which returns the `ResultActions`. Using this result, we can have assertion expectations about the response, like its content, HTTP status, or header.

## Things I want to know more about

1. Not being able to test the entire stack for HTTP requests seems pretty limiting. Will we be learning the Spring Boot RestTemplate to test the app?
