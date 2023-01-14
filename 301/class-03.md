# Reading

[React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?

    An array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    You loop through the array using the `map()` function. Then you return whatever element you want for each iteration, or you assign the mapped array to a variable and display it as the return function.

3. Each list item needs a unique ____.

    key

4. What is the purpose of a key?

    Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?

    The spread (...) syntax allows an iterable, such as an array or string, to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected.

2. List 4 things that the spread operator can do.

    - Copying an array
    - Concatenating or combining arrays
    - Using Math functions
    - Using an array as arguments
    - Adding an item to a list
    - Adding to state in React
    - Combining objects
    - Converting NodeList to an array

3. Give an example of using the spread operator to combine two arrays.

    ```JavaScript
    const arrayOne = [0, 1, 2];
    const arrayTwo = [3, 4, 5];
    const arrayThree = [...arrayOne, ...arrayTwo];
    ```

4. Give an example of using the spread operator to add a new item to an array.

    ```JavaScript
    const arrayOne = [0, 1, 2];
    const arrayTwo = [3, 4, 5, ...arrayOne];
    ```

5. Give an example of using the spread operator to combine two objects into one.

    ```JavaScript
    const objectOne = {foo: bar};
    const objectTwo = {hello: world};
    const objectThree = {
            ...objectOne,
            ...objectTwo,
            };
    ```

## Videos

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?

    Create the function at the level of the state that we're interested in changing.

2. In your own words, what does the increment function do?

    The function takes in a name and iterates over the people array, incrementing the count property of the corresponding person. The return value of the map function is then assigned to the `setState` method to update the people state.

3. How can you pass a method from a parent component into a child component?

    You pass it as a prop like any other prop.

4. How does the child component invoke a method that was passed to it from a parent component?

    By calling `this.props.function()` within the component.

## Bookmark and Review

[React Tutorial through 'Declaring a Winner'](https://reactjs.org/tutorial/tutorial.html)

[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

## Things I want to know more about

1. That [paper](https://grfia.dlsi.ua.es/ml/algorithms/references/editsurvey_bille.pdf) in the reconciliation discussion about React's re-rendering of the DOM is goals. I want to understand it. It's complete gibberish to me, and it makes me miss a time in my life when I was taking vector calc/diff eq/all kinds of physics related to aerodynamics and the like. I want my brain to be that agile again.
