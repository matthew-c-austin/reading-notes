# Reflections

This reading was a lot longer than the others so far, likely because it packs a lot of new (to me) concepts in. I didn't really appreciate the wording in the final reading. It was constantly calling out the reader saying oh I bet you think this is so simple, when in my case it was the first time I saw it. A little disheartening as a comparison against other people in the field looking for employment.

## Reading

[Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

1. Explain why we need domain modeling.

    Domain modeling that's articulated well can verify and validate understanding of a problem domain. The domain is the target subject area of a computer program, and we need some way of defining it. This model describes various entities, their attributes and behaviuors, as well as the constrains that govern the problem. It is a way of level setting that creates a vocabulary that can be used by both technical and business teams.

[HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)

1. Why should tables not be used for page layouts?

    They reduce accessibility for visually impaired users, they produce tag soup, and they are not automatically responsive.

2. List and describe 3 different semantic HTML elements used in an HTML `<table>`.

    `<td>` is a table data element, i.e. a cell in the table
    `<tr>` is a table row, where each `<td>` is placed
    `<th>` is a table header, which is the first row header that makes it easier to find data we're looking for, and they also make tables more accessible to screen readers by associating all data in the column with the header.

[Introducing Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

1. What is a constructor and what are some advantages to using it?

    A constructor is just a function called by using the `new` keyword. When you call a constructor, it will:

    - create a new object
    - bind `this` to the new object, so you can refer to `this` in your constructor code
    - run the code in the constructor
return the new object.

2. How does the term this differ when used in an object literal versus when used in a constructor?

    In an object literal `this` refers to the current object in question. In a constructor `this` refers to the constructor, which can be used to refer to this when creating an new instance of an object with that constructor.

[Object Prototypes Using a Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

1. Explain prototypes and inheritance via an analogy from your previous work experience.
    - NOTE: This is a very common front end developer interview question

    If we were to model a new twin aisle aircraft, say the 777-9, it would be made up of many different parts. We could think of these as objects. For now let's say a fuselage and two wings. These wings and this fuselage are all part of a Boeing twin aisle *airplane*, which all contain some aspects in common.

     Relating to objects and inheritance and prototypes, we'd say that the *fuselage* object and the *wing* objects inherit prototypical properties of an *airplane*, but they may have their own features that are specific to the 777-9, such as composite wings or higher cabin pressure.

## Things I want to know more about

1. In the domain modeling portion, why do we use a function expression to define the EpicFailVideo object versus a function declaration? The previous reading constructor function example from MDN used a declaration.
2. The prototype function being used as best practice is confusing to me. Can you not just add the generateRandom function as a method to the object like for a class? Why is it better for speed to do that to a prototype? Is it that the method is saved in memory for later use by other identically-typed objects?
3. In general, should we use prototypes and constructors as defined here for version compatability or classes as a starting point?
