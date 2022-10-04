# Programming with JavaScript

## [Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)

The *control flow* is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or `if...else`, so that different code executes depending on whether the form is complete or not:

```javascript
if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}
```

A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.

Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

## [Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

### Defining Functions

A **function definition** (also called a **function declaration**, or **function statement**) consists of the function keyword, followed by:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, `{ /* … */ }`.

For example, the following code defines a simple function named square:

```javascript
function square(number) {
  return number * number;
}
```

The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:

```javascript
return number * number;
```

Parameters are essentially passed to functions by value — so if the code within the body of a function assigns a completely new value to a parameter that was passed to the function, the change is not reflected globally or in the code which called that function.

### Function Expressions

While the function declaration above is syntactically a statement, functions can also be created by a function expression.

Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:

```javascript
const square = function (number) {
  return number * number;
}
const x = square(4); // x gets the value 16
```

However, a name can be provided with a function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

```javascript
const factorial = function fac(n) {
  return n < 2 ? 1 : n * fac(n - 1);
}

console.log(factorial(3))
```

A **method** is a function that is a property of an object.

### Calling a Function

Functions must be in scope when they are called, but the function declaration can be hoisted (appear below the call in the code)

The scope of a function is the function in which it is declared (or the entire program, if it is declared at the top level).

There are other ways to call functions. There are often cases where a function needs to be called dynamically, or the number of arguments to a function vary, or in which the context of the function call needs to be set to a specific object determined at runtime.

It turns out that functions are themselves objects — and in turn, these objects have methods. (See the `Function` object.) The `call()` and `apply()` methods can be used to achieve this goal.

## Additional Resources

[Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
