# Read: Class 03

## Reflections

This reading assignment talks about some of the subtleties with primitives versus object wrapped references to those primitives. Exception handling is also discussed at a high level, along with the Scanner object, which breaks down formatted input into tokens and translates those tokens according to their data type.

## Readings

[Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

1. Explain the difference between an “int” and an “Integer” in Java.

    In Java, `int` and `Integer` are related but different data types.

    `int` is a primitive data type that represents a whole number. It is a 32-bit signed two's complement integer, which means it can hold values ranging from -2,147,483,648 to 2,147,483,647.

    On the other hand, `Integer` is a class in the Java language's standard library that provides an object representation of an `int` value. It wraps an `int` value in an object, allowing it to be used in situations where an object is required, such as in a collection. `Integer` provides many useful methods for working with int values, such as `parseInt()` for converting a string to an int.

    One key difference between `int` and `Integer` is that `int` is a primitive data type, while `Integer` is a class. As a result, `int` values can be assigned directly to variables and used in expressions, while `Integer` values must be created using the `new` keyword and treated as objects.

2. What is the default value for ints? Integers?

   `0` for `int` and `null` for `Interger`

3. What is autoboxing? Unboxing?

    The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

[Exceptions in Java](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

1. List the three basic categories of exceptions.

    - **Checked Exception** - These are exceptional conditions that a well-written application should anticipate and recover from. Checked exceptions *are subject* to the Catch or Specify Requirement. All exceptions are checked exceptions, except for those indicated by `Error, RuntimeException`, and their subclasses.
    - **Error** - These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from. Errors are *not subject* to the Catch or Specify Requirement. Errors are those exceptions indicated by `Error` and its subclasses.
    - **Runtime Exception** - These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from. These usually indicate programming bugs, such as logic errors or improper use of an API. Runtime exceptions are *not subject* to the Catch or Specify Requirement. Runtime exceptions are those indicated by `RuntimeException` and its subclasses. Errors and runtime exceptions are collectively known as *unchecked exceptions*.

2. What type of statement can you use to handle an exception?

    ```Java
    try {
        code
    }
    catch and finally blocks . . .
    ```

[Using Scanner to read in a file in Java](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)

1. Describe a situation where you think it would be useful to have a program that scans text.

    A plagiarism detector or spam filtering

2. What is input from a Scanner broken down into?

    Tokens

## Things I want to know more about

1. How would you check if a value has been initialized in the case of a primitive vs. just that it is equal to the default value?
2. What is the most common Java version used in the industry today?
3. I noticed the scanner tutorial didn't use the `try-with-resources` methodology. Is it the general case that Java tutorials use older version functionality in their examples rather than blanket best practices introduced in later versions?
