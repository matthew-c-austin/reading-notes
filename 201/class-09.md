# Reflections

This reading was about web forms and events, two pivotal concepts in web development. There's a deep ocean of UX theory on how to style and create web forms. There's a crazy impossible amount of event handlers in any given web application. This felt like looking at the sun. There's a lot to take in and it's painful to consider for too long.

## Reading

[HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

[Your First Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)

[How to Structure a Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

1. Why are forms so important in web development?

    Web forms are one of the main points of interaction between a user and a site or application. It allows them to enter data, which can be used in a variety of ways.

2. When designing a form, what are some key things to keep in mind when it comes to user experience?

    - The bigger your form, the more you risk frustrating people and losing users.
    - Keep it simple and stay focused.Only ask for data you absolutely need.
    - Labels should be clear and visible and work without context.

3. List 5 form elements and explain their importance.

    1. The `<form>` element formally defines a forma nd attributes that determine the form's behavior. It is the base element of a form.
    2. The `<fieldset>` element is a convenient way to create groups of widgets that share the same purpose for styling and semantic purposes.
    3. The `<legend>` is an element just below the opening of a `<fieldset>` element whose text describes the labels. It's used by assistive technologies.
    4. A `<label>` element is the formal way to define a label for an HTML form widget.his is the most important element if you want to build accessible forms.
    5. The `<input>` HTML element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent. The `<input>` element is one of the most powerful and complex in all of HTML due to the sheer number of combinations of input types and attributes.

[Learn JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

[Introduction to Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1. How would you describe events to a non-technical friend?

    Events are just things that happen. In the context of coding and web development, it's generally stuff happening on the webpage that can be reacted to, like clicking with a mouse or typing or pressing enter on a button.

2. When using the `addEventListener()` method, what 2 arguments will you need to provide?

    Inside the `addEventListener()` function, we specify two parameters: the name of the event we want to register this handler for, and the code that comprises the handler function we want to run in response to it.

3. Describe the event object. Why is the target within the event object useful?

    The event object has extra features and properties and refers to the event itself. These can be useful depending on what you're trying to do.

4. What is the difference between event bubbling and event capturing?

    Event bubbling is how all modern browsers by default handle event listeners. It registers some event (say a click) in an element if the target has an event handler, then it checks each subsequent ancestor. This happens AFTER the capturing phase, which goes outward-in (ancestor to children to the eventual target).

## Things I want to know more about

1. The idea of event bubbling is confusing to me. Why do browsers use bubbling phase by default for event handlers?
