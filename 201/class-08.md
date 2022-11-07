# Reflections

This reading was about CSS flexbox. To be honest I can see the information and grasp the idea of the flexbox, but I really don't know when to apply it as a rule.

## Reading

[Learn CSS - Flexbox](https://web.dev/learn/css/flexbox/)

1. Flexbox is designed for one-dimensional content. Explain what this means.

    In this case, one-dimensional is content arranged in columns *or* rows. It excels at taking a bunch of items which have different sizes, and returning the best layout for those items.

    In terms of space distribution, each line acts like a new flex container. Therefore if you are wrapping rows, it is not possible to get something in row 2 to line up with something above it in row 1. This is what is meant by flexbox being one-dimensional. You can control alignment in one axis, a row or a column, not both together as we can do in grid.

2. Explain the difference between the main axis and cross axis.

    The main axis is set by the `flex-direction` property. It can be a `row` or `column`. Flex items move as a group on the main axis. The cross axis is orthogonal to the main axis. You can move items individually or as a group so the align against each other and the flex container on the cross axis.

3. How can using certain properties of flexbox negatively impact accessibility?

    Things like `row-reverse` and `column-reverse` only reorder the visual disply and not the logical order. Therefore screen readers won't read out the data the way it is displayed on the screen, which makes it difficult to follow.

[CSS Layout - Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

1. What are some advantages of using flexbox over float?

    With float, the following simple layout designs are either difficult or impossible to achieve with such tools in any kind of convenient, flexible way:

    - Vertically centering a block of content inside its parent.
    - Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
    - Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

2. How does this topic connect with your long term goals?

    I suppose it's another tool in the toolbox for website design and layout, but honestly I just don't get when you'd make the choice to use it, and what the best practices are for it.

## Things I want to know more about

1. When would you use flexbox versus grid?
