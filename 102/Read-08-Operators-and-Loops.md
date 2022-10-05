# Operators and Loops

## [Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

At a high level, an *expression* is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.

All complex expressions are joined by operators, such as = and +. In this section, we will introduce the following operators.

### Assignment Operators

| Name                           | Shorthand operator   | Meaning             |
|--------------------------------|----------------------|---------------------|
| Assignment                     |  x = f()             | = f()               |
| Addition assignment            |  x += f()            | = x + f()           |
| Subtraction assignment         |  x -= f()            | = x - f()           |
| Multiplication assignment      |  x *= f()            | = x * f()           |
| Division assignment            |  x /= f()            | = x / f()           |
| Remainder assignment           |  x %= f()            | = x % f()           |
| Exponentiation assignment      |  x **= f()           | = x ** f()          |
| Left shift assignment          |  x <<= f()           | = x << f()          |
| Right shift assignment         |  x >>= f()           | = x >> f()          |
| Unsigned right shift assignment|  x >>>= f()          | = x >>> f()         |
| Bitwise AND assignment         |  x &= f()            | = x & f()           |
| Bitwise XOR assignment         |  x ^= f()            | = x ^ f()           |
| Bitwise OR assignment          |  x \|= f()           | = x \| f()          |
| Logical AND assignment         |  x &&= f()           | && (x = f())        |
| Logical OR assignment          |  x \|\|= f()         | \|\| (x = f())      |
| Logical nullish assignment     |  x ??= f()           | ?? (x = f())        |

If an expression evaluates to an **object**, then the left-hand side of an assignment expression may make assignments to properties of that expression.

### Comparison Operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality.

| Operator                   | Description                                                                                         | Examples returning true       |
|----------------------------|-----------------------------------------------------------------------------------------------------|-------------------------------|
| Equal (==)                 | Returns true if the operands are equal.                                                             | 3 == var1 "3" == var13 == '3' |
| Not equal (!=)             | Returns true if the operands are not equal.                                                         | var1 != 4 var2 != "3"         |
| Strict equal (===)         | Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS. | 3 === var1                    |
| Strict not equal (!==)     | Returns true if the operands are of the same type but not equal, or are of different type.          | var1 !== "3" 3 !== '3'        |
| Greater than (>)           | Returns true if the left operand is greater than the right operand.                                 | var2 > var1 "12" > 2          |
| Greater than or equal (>=) | Returns true if the left operand is greater than or equal to the right operand.                     | var2 >= var1 var1 >= 3        |
| Less than (<)              | Returns true if the left operand is less than the right operand.                                    | var1 < var2 "2" < 12          |
| Less than or equal (<=)    | Returns true if the left operand is less than or equal to the right operand.                        | var1 <= var2 var2 <= 5        |

### Arithmetic Operators

An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`). These operators work as they do in most other programming languages when used with floating point numbers (in particular, note that division by zero produces `Infinity`).

| Operator                     | Description                                                                                                                                                                                                              | Example                                                                                           |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| Remainder (%)                | Binary operator. Returns the integer remainder of dividing the two operands.                                                                                                                                             | 12 % 5 returns 2.                                                                                 |
| Increment (++)               | Unary operator. Adds one to its operand. If used as a prefix operator (++x), returns the value of its operand after adding one; if used as a postfix operator (x++), returns the value of its operand before adding one. | If x is 3, then ++x sets x to 4 and returns 4, whereas x++ returns 3 and, only then, sets x to 4. |
| Decrement (--)               | Unary operator. Subtracts one from its operand. The return value is analogous to that for the increment operator.                                                                                                        | If x is 3, then --x sets x to 2 and returns 2, whereas x-- returns 3 and, only then, sets x to 2. |
| Unary negation (-)           | Unary operator. Returns the negation of its operand.                                                                                                                                                                     | If x is 3, then -x returns -3.                                                                    |
| Unary plus (+)               | Unary operator. Attempts to convert the operand to a number, if it is not already.                                                                                                                                       | +"3" returns 3. +true returns 1.                                                                  |
| Exponentiation operator (**) | Calculates the base to the exponent power, that is, base^exponent                                                                                                                                                        | 2 ** 3 returns 8. 10 ** -1 returns 0.1.                                                           |

## [Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

```javascript
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
```

There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!)

The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.

The statements for loops provided in JavaScript are:

- for statement
- do...while statement
- while statement
- labeled statement
- break statement
- continue statement
- for...in statement
- for...of statement

### for statement

A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

A for statement looks as follows:

```javascript
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```

When a `for` loop executes, the following occurs:

1. The initializing expression `initialExpression`, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The `conditionExpression` expression is evaluated. If the value of `conditionExpression` is true, the loop statements execute. Otherwise, the for loop terminates. (If the `conditionExpression` expression is omitted entirely, the condition is assumed to be true.)
3. The `statement` executes. To execute multiple statements, use a **block statement** (`{ }`) to group those statements.
4. If present, the update expression incrementExpression is executed.
5. Control returns to Step 2.

### while statement

A `while` statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

```javascript
while (condition)
  statement
```

If the `condition` becomes `false`, `statement` within the loop stops executing and control passes to the statement following the loop.

The condition test occurs *before* `statement` in the loop is executed. If the condition returns `true`, `statement` is executed and the condition is tested again. If the condition returns `false`, execution stops, and control is passed to the statement following `while`.

To execute multiple statements, use a block statement (`{ }`) to group those statements.
