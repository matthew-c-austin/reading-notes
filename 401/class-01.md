# Read: Class 01

## Reflections

This reading assignment introduces compilation as a concept, as well as the primitive data types in Java, strongly typed languages, and some basic functionality in Java related to keywords and console logging.

## Readings

[Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

1. What does “strong typed” mean?

    The programming language requires a specific data type assigned to each variable, and the compiler/interpreter checks that the operations performed on the variable are appropriate for that data type.

2. What are the primitive data types?

    - **byte**: The `byte` data type is an 8-bit signed two's complement integer. It has a minimum value of -128 and a maximum value of 127 (inclusive). The byte data type can be useful for saving memory in large arrays, where the memory savings actually matters. They can also be used in place of `int` where their limits help to clarify your code; the fact that a variable's range is limited can serve as a form of documentation.

    - **short**: The `short` data type is a 16-bit signed two's complement integer. It has a minimum value of -32,768 and a maximum value of 32,767 (inclusive). As with `byte`, the same guidelines apply: you can use a `short` to save memory in large arrays, in situations where the memory savings actually matters.

    - **int**: By default, the `int` data type is a 32-bit signed two's complement integer, which has a minimum value of -2<sup>31<sup> and a maximum value of 2<sup>31<sup>-1. In Java SE 8 and later, you can use the `int` data type to represent an unsigned 32-bit integer, which has a minimum value of 0 and a maximum value of 2<sup>32<sup>-1. Use the Integer class to use int data type as an unsigned integer. See the section The Number Classes for more information. Static methods like compareUnsigned, divideUnsigned etc have been added to the Integer class to support the arithmetic operations for unsigned integers.

    - **long**: The `long` data type is a 64-bit two's complement integer. The signed `long` has a minimum value of -2<sup>63<sup> and a maximum value of 2<sup>63<sup>-1. In Java SE 8 and later, you can use the `long` data type to represent an unsigned 64-bit `long`, which has a minimum value of 0 and a maximum value of 2<sup>64<sup>-1. Use this data type when you need a range of values wider than those provided by `int`. The `Long` class also contains methods like `compareUnsigned`, `divideUnsigned` etc to support arithmetic operations for unsigned long.

    - **float**: The `float` data type is a single-precision 32-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. As with the recommendations for `byte` and `short`, use a `float` (instead of `double`) if you need to save memory in large arrays of floating point numbers. This data type should never be used for precise values, such as currency. For that, you will need to use the `java.math.BigDecimal` class instead. Numbers and Strings covers `BigDecimal` and other useful classes provided by the Java platform.

    - **double**: The `double` data type is a double-precision 64-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the Floating-Point Types, Formats, and Values section of the Java Language Specification. For decimal values, this data type is generally the default choice. As mentioned above, this data type should never be used for precise values, such as currency.

    - **boolean**: The `boolean` data type has only two possible values: `true` and `false`. Use this data type for simple flags that track true/false conditions. This data type represents one bit of information, but its "size" isn't something that's precisely defined.

    - **char**: The `char` data type is a single 16-bit Unicode character. It has a minimum value of `'\u0000'` (or 0) and a maximum value of `'\uffff'` (or 65,535 inclusive).

[The first response in this Reddit thread on compiling](https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)

[XKCD: Compiling](https://xkcd.com/303/)

1. Explain to a non-technical friend the difference in how compilation works in Java and JavaScript.

    The abstraction of more natural language that the developer uses needs to be translated to something the computer can read, i.e., 1's and 0's. In Java, and in other compiled languages, this translation happens before the program is run. In JavaScript, and other interpreted languages, this process happens in real-time. Since this obviously takes time, it's something that can slow performance for languages like JavaScript.

    Compilation also checks for "rule-following" that, if left unaddressed, can cause errors in the execution of the program. In general, compiling is an upfront time sink that leads to safer code that runs faster, but interpreted code is quicker to iterate on and get out the door.

2. Does code complining mean that it works correctly?

    No, only that the program follows the rules of the language. You can still make errors in the code that produce unintended behavior.

[Reading Java Documentation](https://www.dummies.com/category/articles/java-33602/)

1. How many keywords does Java have?

    As of Java 16, Java has 57 keywords. Here is the list of Java keywords:

    ```Java
    abstract, assert, boolean, break, byte, case, catch, char, class, const (not used), continue, default, do, double, else, enum, exports (added in Java 9), extends, false, final, finally, float, for, goto (not used), if, implements, import, instanceof, int, interface, long, module (added in Java 9), native, new, null, opens (added in Java 9), package, private, protected, provides (added in Java 9), public, requires (added in Java 9), return, short, static, strictfp, super, switch, synchronized, this, throw, throws, transient, true, try, var (added in Java 10), void, volatile, while, with (added in Java 14)
    ```

    It's worth noting that some keywords, such as const and goto, were reserved in earlier versions of Java but are not used in the current version. Additionally, some keywords such as var, module, requires, opens, provides, and with were added in more recent versions of Java.

2. How do you print words to the console in Java?

    ```Java
    System.out.println("Some string");
    ```

## Things I want to know more about

1. Why is it that a boolean's size isn't precisely defined in Java? Does the compiler leave it up to the O/S or CPU to determine how much space it takes up in memory?
