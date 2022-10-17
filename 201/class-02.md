# Reflections

This reading digs deeper into the basics of HTML, CSS, and JavaScript. For HTML we learn about several more tags, as well as the importance of semantic elements.

For CSS we learn about how to avoid inline styling, as well as some of the terminology for the structure of CSS (selector, declarations, properties, values)

For JavaScript we learn about comparison operators in detail, as well as general operators

## Learn HTML

[Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)

[HTML Text Fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

[HTML Advanced Text Formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

1. Why is it important to use semantic elements in our HTML?

    Semantic elements are used by search engine for SEO and screen readers for the visually impaired. They make it easier to find blocks of meaningful code, and suggest to the developer the type of data that will be populated. In addition, it makes it easier to target content effectively with CSS styling or JavaScript.

2. How many levels of headings are there in HTML?

    6

3. What are some uses for the `<sup>` and `<sub>` elements?

    Ordinal numbering, mathematical expressions, chemical formulas, footnotes, etc.

4. When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

    `title`

## Learn CSS

[How CSS is Structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

1. What are ways we can apply CSS to our HTML?

    1. External style sheet contained in a separate file with a `.css` extension. This is the most common and useful method of bringing CSS to a document.

    2. An internal stylesheet that resides within the HTML document, created inside a `<style>` element inside the HTML `<head>`.

    3. Inline styling with CSS declarations that affect a sing HTML element, contained within a `style` attribute.

2. Why should we avoid using inline styles?

    It's the least efficient implementation, it mixes presentational code with HTML and content, making it more difficult to read and understand.

3. Review the block of code below and answer the following questions:

    1. What is representing the selector?

        h2

    2. Which components are the CSS declarations?

        ```CSS
        {
            color: black;
            padding: 5px;
        } 
        ```

    3. Which components are considered properties?

        color, padding

    ```CSS
    h2 {
        color: black;
        padding: 5px;
    } 
    ```

## Learn JS

[JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

1. What data type is a sequence of text enclosed in single quote marks?

    String

2. List 4 types of JavaScript operators.

    | Operator                              | Explanation                                                                                                                                                                                                       | Symbol(s) | Example                                                                                                                                                                                                                                                                                                                                                         |
    |---------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Addition                              | Add two numbers together or combine two strings.                                                                                                                                                                  | +         | 6 + 9; 'Hello ' + 'world!';                                                                                                                                                                                                                                                                                                                                     |
    | Subtraction, Multiplication, Division | These do what you'd expect them to do in basic math.                                                                                                                                                              | -, *, /   | 9 - 3; 8 * 2; // multiply in JS is an asterisk 9 / 3;                                                                                                                                                                                                                                                                                                           |
    | Assignment                            | As you've seen already: this assigns a value to a variable.                                                                                                                                                       | =         | let myVariable = 'Bob';                                                                                                                                                                                                                                                                                                                                         |
    | Strict equality                       | This performs a test to see if two values are equal. It returns a true/false (Boolean) result.                                                                                                                    | ===       | let myVariable = 3; myVariable === 4;                                                                                                                                                                                                                                                                                                                           |
    | Not, Does-not-equal                   | This returns the logically opposite value of what it precedes. It turns a true into a false, etc.. When it is used alongside the Equality operator, the negation operator tests whether two values are not equal. | !, !==    | For "Not", the basic expression is true, but the comparison returns false because we negate it: let myVariable = 3; !(myVariable === 3); "Does-not-equal" gives basically the same result with different syntax. Here we are testing "is myVariable NOT equal to 3". This returns false because myVariable IS equal to 3: let myVariable = 3; myVariable !== 3; |

3. Describe a real world problem you could solve with a Function.

    You could find the nth number fibonacci sequence, or replace every 3rd index in an array with 'fizz'. You know, real world stuff.

[Making Decisions in your Code - Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

1. An if statement checks a **condition** and if it evaluates to ``true``, then the code block will execute.

2. What is the use of an `else if` statement?

    Add aditional choices/outcomes beyond the two that `if...else` provides.

3. List 3 different types of comparison operators.

    | Operator | Name                     | Purpose                                                                  | Example      |
    |----------|--------------------------|--------------------------------------------------------------------------|--------------|
    | ===      | Strict equality          | Tests whether the left and right values are identical to one another     | 5 === 2 + 4  |
    | !==      | Strict-non-equality      | Tests whether the left and right values are not identical to one another | 5 !== 2 + 3  |
    | <        | Less than                | Tests whether the left value is smaller than the right one.              | 10 < 6       |
    | >        | Greater than             | Tests whether the left value is greater than the right one.              | 10 > 20      |
    | <=       | Less than or equal to    | Tests whether the left value is smaller than or equal to the right one.  | 3 <= 2       |
    | >=       | Greater than or equal to | Tests whether the left value is greater than or equal to the right one.  | 5 >= 4       |

4. What is the difference between the logical operator `&&` and `||`?

    - For `&&` - AND; you chain together two or more expressions so that all of them have to individually evaluate to `true` for the whole expression to be `true`.
    - For `||` - OR; allows you to chain together two or more expressions so that one or more of them have to individually evaluate to `true` for the whole expression to return `true`.

## Things I want to know more about

1. Is there any reason you wouldn't use strict equality? Just as a way to prevent trouble with an already dynamic and weakly typed language.
