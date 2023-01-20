# Reading

[React Docs - Forms](https://reactjs.org/docs/forms.html)

1. What is a ‘Controlled Component’?

    A controlled component is a React component which uses state to be the "single source of truth" within some HTML form element that typically maintain their own state and update it based on user input. Then the React component that renders a form also controls what happens in that form on subsequent user input.

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?

    We should do it on change to the input field, as we might want to use that information before a submit event to indicate invalid inputs or for autofill or other functionality that precedes the submit event.

3. How do we target what the user is entering if we have an event handler on an input field?

    With setting the `value` attribute to the `this.state.relevantState`, as well as having an `onChange` event handler, as noted above.

[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

1. Why would we use a ternary operator?

    For simple conditionals it reduces code bloat.

2. Rewrite the following statement using a ternary statement:

```JavaScript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

```JavaScript
x===y ? console.log(true) : console.log(false);
```

## Bookmark and Review

[React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)

[React Docs - Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

## Things I want to know more about

1. Is it more common to use the ternary or short circuit evaluation in React?
