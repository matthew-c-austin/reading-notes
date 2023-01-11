# Reading

[React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

    render

2. What is the very first thing to happen in the lifecycle of React?

    the mounting phase (constructor being the first step)

3. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`

    - `constructor`
    - `render`
    - `componentDidMount`
    - `React Updates`
    - `componentWillUnmount`

4. What does componentDidMount do?

    `componentDidMount()` is invoked immediately after a component is mounted (inserted into the tree). Initialization that requires DOM nodes should go here. If you need to load data from a remote endpoint, this is a good place to instantiate the network request.

    This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in `componentWillUnmount()`.

## Videos

[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?

    Initialized values of properties ala html properties (title/src/description/anything you want to handle inside the component)

2. What is the big difference between props and state?

    Props is passed into a component and state is handled within the component

3. When do we re-render our application?

    When the state is changed

4. What are some examples of things that we could store in state?

    Anything in a form

## Bookmark and Review

[React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

[React Docs - handling events](https://reactjs.org/docs/handling-events.html)

[React Tutorial through 'Developer Tools'](https://reactjs.org/tutorial/tutorial.html)

[React Bootstrap Documentation](https://react-bootstrap.github.io/)

[Bootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)

[Bootstrap Shuffle - a class "sandbox"](https://bootstrapshuffle.com/classes)

[Netlify](https://www.netlify.com/)

## Things I want to know more about

1. I note that we're learning the class definition of components instead of hooks. Will we be learning hooks as well?
