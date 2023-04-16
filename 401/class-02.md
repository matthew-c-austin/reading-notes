# Read: Class 02

## Reflections

This reading assignment introduces Java packages, as well as some basic discussion on loops and arrays. As with all of these early assignments, these are foundational building blocks needed to be able to program in Java.

## Readings

[Java Imports](https://www.programiz.com/java-programming/packages-import)

1. Use an analogy to explain Built-In packages. Give examples.

    Java Built-In packages can be thought of as toolboxes filled with pre-built tools that Java programmers can use to create their programs. Just as a mechanic might have different toolboxes filled with different sets of tools for different types of repairs, Java has different built-in packages with different sets of classes and utilities for different types of programming tasks.

    For example, the `java.util` package contains tools for working with collections, such as lists and maps, while the `java.io` package contains tools for input and output, such as reading and writing files.

2. Explain the steps for creating a new package in IntelliJ.

    In IntelliJ IDEA, here's how you can create a package:

    1. Right-click on the source folder.

    2. Go to new and then package.

    3. A pop-up box will appear where you can enter the package name.

    Once the package is created, a similar folder structure will be created on your file system as well. Now, you can create classes, interfaces, and so on inside the package.

[Different types of loops in Java](https://www.baeldung.com/java-loops)

1. Which loop types use a loop counter?

    A `for` loop

2. Explain the difference between While and Do-While loops.

    A *while* loop repeats a block of code *while* the controlling boolean-expression is `true`. This expression is evaluated at the beginning of the loop, before the code block is executed.

    A *do-while* loop differs in that the expression is evaluated at the end of the block. The bottom line is that if you want to do something at least once, you'd use a *do-while* loop.

[Java Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)

1. Describe 3 built-in methods for Arrays.

    1. `Arrays.binarySearch()`: This method is used to search for a specific element in a sorted array. It takes the sorted array and the element to search for as arguments and returns the index of the element if it's found, or a negative value if it's not found. Note that the `binarySearch()` method requires that the array be sorted in ascending order, otherwise the result may be incorrect.

    2. `Arrays.equals()`: Returns true if the two specified arrays of longs are equal to one another. Two arrays are considered equal if both arrays contain the same number of elements, and all corresponding pairs of elements in the two arrays are equal. This returns true if the two arrays are equal. Same method could be used by all other primitive data types (Byte, short, Int, etc.)

    3. `Arrays.fill()`: This method is used to fill an array with a specific value. It takes the array to fill, the starting index, the ending index, and the value to fill with as arguments.

    4. `Arrays.sort()`: This method is used to sort the elements of an array in ascending order. It takes the array as an argument and returns the sorted array.

2. How is the size of an array determined in Java?

    In Java, the size of an array is determined at the time of its creation and cannot be changed afterward. To create an array with a specific size, you can specify the size when you declare the array using square brackets, like this:

    ```Java
    int[] myArray = new int[10];
    ```

    You can also initialize an array with values at the time of creation

    ```Java
    int[] myArray = {1, 2, 3, 4, 5};
    ```

## Things I want to know more about

1. Is it best practice to use imports at the top of the Class rather than using the fully qualified name within the code?
2. How does `Arrays.equals()` treat indices with objects as values? Is it a deeply equals method, or will it only return true if they are the same object?
