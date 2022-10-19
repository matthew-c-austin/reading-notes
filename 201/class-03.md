# Reflections

This reading introduced the conpcept of the box model in CSS, which defines how parts of a box - margin, border, padding, and content - work together together to create a box that you can see on a page. It's relatively confusing how behvaior changes depending on types of boxes/properties within those boxes, and it's something that is necessary to understand for mastery of CSS.

The JavaScript portion expanded on the concept of an array, as well as showing that an array of arays is a valid array. In addition, some of the nuance of type conversion performed automatically in JavaScript is explored.

## [Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

[Ordered](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML) and [Unordered](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul) lists

1. When should you use an `unordered list` in your HTML document?

    Typically for grouping a collection of items that do not have a numerical order, i.e. their order in the list is meaningless.

2. How do you change the `bullet style` of unordered list items?

    Using the `list-style-type` property in CSS

3. When should you use an `ordered list` vs an `unordered list` in your HTML document?

    Whenever order is meaningful. Examples such as steps in a recipe, turn-by-turn diretions, or a list of ingredients in nutrition information lables with decreasing proportion all care about the order of the list.

4. Describe two ways you can change the numbers on `list items` provided by an `ordered list`?

    Using the `reversed` attribute will number the items from high to low. Or the `start` attribute set to some number begins the list at that number, like `start="4"`. If you want to change the type you can use the `type` attribute.

## [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

[The Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

1. Describe the CSS properties of `margin` and `padding` as characters in a story. What is their role in a story titled: “The Box Model”?

    "I am `margin`. Cannon fodder. Expendable. First to fight. First to die. I stand outside the `border`, giving my life for p*recious* `content`."

    "I am `padding`. The honor guard, the last line of defense. When margin has fallen and border is a memory, I'm all that stands between `content` and ruin."

2. List and describe the **four** parts of an HTML elements box as referred to by the `box model`.

    - **Content box**: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
    - **Padding box**: The padding sits around the content as white space; size it using padding and related properties.
    - **Border box**: The border box wraps the content and any padding; size it using border and related properties.
    - **Margin box**: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.

## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

[Arrays](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays)

[Operators and Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

[Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)

[Loops](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)

1. What `data types` can you store inside of an `Array`?

    You can store strings, numbers, objects, and other arrays. Data types can be mixed in a single array.

2. Is the `people` array a valid JavaScript array? If so, how can I access the values stored? If not, why?

    The `people` array is a valid JS array. You can access the values with

    ```JavaScript
    people[i][j];
    ```

    where `i` and `j` are indices of the first and second level arrays, respectively

    ```Javascript
    const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
    ```

3. List **five** shorthand operators for assignment in javascript and describe what they do.

    | Name                      | Shorthand operator | Meaning     |
    |---------------------------|--------------------|-------------|
    | Addition assignment       | x += f()           | x = x + f() |
    | Subtraction assignment    | x -= f()           | x = x - f() |
    | Multiplication assignment | x *= f()           | x = x * f() |
    | Division assignment       | x /= f()           | x = x / f() |
    | Remainder assignment      | x %= f()           | x = x % f() |

4. Read the code below and evaluate the last expression and explain what the result would be and why.

    The result would be `10dog`. This is because when adding `a + c`, `false` is equivalent to `0`, so

    ```javascript
    (10 + 0) == 10.
    ```

    Next, the `number` `10` is concatenated with the value of `b`, which is the `string` `"dog"`. If `c` were to equal `true`, then the expression would equal `11dog`.

    ```javascript
    let a = 10;
    let b = 'dog';
    let c = false;

    // evaluate this
    (a + c) + b;
    ```

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

    If you're pulling testimonials or reviews from an API on an infinite scroll page, you want to see if you've reached the end of the entries, which presumably has some parameter like `hasNext`.

6. Give an example of when a Loop is useful in JavaScript.

    From the example above, you might need to loop through all the review strings you've pulled from the API call to add each to the DOM.

## Things I want to know more about

1. The CSS box model and the different applications of padding/border/margin are opaque to me. Is there a reason to choose margin vs. border, for instance? Do you need both?
