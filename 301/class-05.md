# Reading

[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the `single responsibility principle` and how does it apply to components?

    The **single-responsibility principle (SRP)** is a computer programming principle that states that "A module should be responsible to one, and only one, actor." As relates to React, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

    A version that has no interactivity, i.e. no *state*. You can build top-down or bottom-up. In simpler examples, it’s usually easier to go top-down, and on larger projects, it’s easier to go bottom-up and write tests as you build.

3. Once you have a static application, what do you need to add?

    state

4. What are the three questions you can ask to determine if something is state?

    1. Is it passed in from a parent via props? If so, it probably isn’t state.
    2. Does it remain unchanged over time? If so, it probably isn’t state.
    3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. How can you identify where state needs to live?

    For each piece of state in your application:

    - Identify every component that renders something based on that state.
    - Find a common owner component (a single component above all the components that need the state in the hierarchy).
    - Either the common owner or another component higher up in the hierarchy should own the state.
    - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?

    Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions. Higher-order functions allow us to abstract over *actions*, not just values.

2. Explore the `greaterThan` function as defined in the reading. In your own words, what is line 2 of this function doing?

    Line 2 returns a function which takes an argument `m` and returns the comparison of `m` to the `greaterThan` parameter `n`.

3. Explain how either `map` or `reduce` operates, with regards to higher-order functions.

   The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function. That is to say, map uses a `transform` function as one of its arguments that modifies each element of an array in some way, and pushes it to a new array.

## Things I want to know more about

1. I was actually really interested in the step-by-step approach outlined the React docs. It was a glance into how these things might be done in a bigger org with a full team or teams working on an entire complicated site. I want to know more about the details of that type of work.
