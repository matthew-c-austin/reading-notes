# Read: Class 12

## Reflections

This reading assignment talks about the Spring Data JPA, and some of the ability for automatically creating implementations of interface methods based off of their name, which is very handy. We are also introduced to some of the repositories and their methods, along with a few pitfalls of using these frameworks

## Readings

[Spring guide: Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)

1. How are query methods defined when using Spring Data JPA?

    Spring Data JPA allows you to define query methods in a repository interface by simply declaring method signatures following a naming convention. The Spring Data JPA framework will automatically generate the implementation of these methods based on the method name, which usually consists of a verb (e.g., find, get, count) followed by optional keywords (e.g., By, And, Or, Is, Not) and property names of the entity.

2. Which dependencies will you need in order to complete the Spring guide?

    In your `build.gradle` file:

    ```Java
    plugins {
        id 'java'
        id 'org.springframework.boot' version '3.0.6'
        id 'io.spring.dependency-management' version '1.1.0'
    }

    group = 'com.example'
    version = '0.0.1-SNAPSHOT'
    sourceCompatibility = '17'

    repositories {
        mavenCentral()
    }

    dependencies {
        implementation 'org.springframework.boot:spring-boot-starter'
        testImplementation 'org.springframework.boot:spring-boot-starter-test'
    }

    tasks.named('test') {
        useJUnitPlatform()
    }
    ```

3. What annotations are used to specify an auto generated identification number for an Entity?

    To specify an auto-generated identification number for an entity in a Spring Data JPA application, you can use the `@Id` and `@GeneratedValue` annotations.

[Baeldung: Comparing repositories](https://www.baeldung.com/spring-data-repositories)

1. Which of the Spring Data Repositories covered in the readings has the most methods available to it?

    `JpaRepository` is the Spring Data Repository that has the most methods available to it. It extends `PagingAndSortingRepository`, which in turn extends `CrudRepository`. This means that `JpaRepository` inherits all the methods available from these two parent repositories, in addition to its own specific methods. By using `JpaRepository`, you get basic CRUD operations, as well as pagination and sorting functionality.

2. Name a downside of a Spring Data Repository.

    Beyond all the very useful advantages of these repositories, there are some basic downsides of directly depending on these as well:

    1. We couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; that's of course not unique to this library – but we do have to be careful not to expose these internal implementation details
    2. By extending e.g. `CrudRepository`, we expose a complete set of persistence method at once. This is probably fine in most circumstances as well but we might run into situations where we'd like to gain more fine-grained control over the methods exposed, e.g. to create a ReadOnlyRepository that doesn't include the `save(…)` and `delete(…)` methods of `CrudRepository`

3. How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

    ```Java
    import org.springframework.data.jpa.repository.JpaRepository;

    public interface StudentRepository extends JpaRepository<Student, Long> {
        List<Student> findByName(String name);
    }
    ```

## Things I want to know more about

1. When do we start talking about SQL and its integration into our apps?
