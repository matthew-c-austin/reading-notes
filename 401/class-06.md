# Read: Class 06

## Reflections

This reading assignment is a review of object-oriented programming concepts in Java, which is important because Java is almost pure OO. Inheritance is covered, as well as Static methods and the Java Singleton Class.

## Readings

[Java OO Tutorial](https://docs.oracle.com/javase/tutorial/java/concepts/)

1. Explain the difference between an object and a class.

    An object is a bundle of related state and behavior in software (fields and methods, nouns and verbs).

2. Explain to a non-technical friend the concept of inheritance in Java.

   Inheritance in Java allows you to create new classes based on existing ones, like a family tree. By using the `extends` keyword, a class can inherit traits and methods from a parent class. This helps to organize code logically, reuse existing code, and make changes that affect all related classes. Inheritance simplifies code management and maintenance by reducing redundancy. Think of it as sharing common traits among a family of related classes.

    ```Java
    class Dog extends Animal {
    // additional Dog-specific traits and methods go here
    }
    ```

[Java Static Keyword](https://www.programiz.com/java-programming/static-keyword)

1. Static methods are also called what? Why?

    Class methods, because these static methods belong to the class rather than the object of a class or an instance of that class.

2. How can you access a variable of a class without instantiating an object from that class?

    To access a variable of a class without creating an object, you can use a static variable. A static variable belongs to the class itself, not to any specific instance of the class. You can access it using the class name followed by a dot (.) and the variable name. Here's an example:

    ```Java
    class MyClass {
        static int myStaticVariable = 10;
    }

    public class Main {
        public static void main(String[] args) {
            // Accessing the static variable without creating an object
            System.out.println(MyClass.myStaticVariable); // Output: 10
        }
    }
    ```

[Java Singleton Class](https://www.programiz.com/java-programming/singleton)

1. What is a Design Pattern? Describe one or two with analogies from your previous work experience.

    A design pattern is a reusable solution to common problems in software design, evolved over time to represent best practices for modularity, maintainability, efficiency, etc.

    As an aerospace engineer, here's an example of the Singleton Pattern: Think of it as the aircraft's flight control computer. There is only one main computer responsible for controlling the entire aircraft's flight systems, and all other subsystems must communicate with this single computer to function correctly.

2. What is a Singleton?

    Singleton Pattern: This design pattern ensures that a class has only one instance and provides a global point of access to it.

## Things I want to know more about

1. How do multiple users access a Singleton?
