# Reflections

Here we begin getting into the fun stuff that I haven't had much exposure to. OOP and the DOM. Let's goooooo!

## Reading

[JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

1. How would you describe an object to a non-technical friend you grew up with?

    An object is just a chunk of data and code. Rather than structure programs separating those two concepts, objects combine them into one.

2. What are some advantages to creating object literals?

    It allows you to transfer a series of structured, related data items in some manner, which can be more efficient and easier to work with than items in an array when you want to individually identify them.

3. How do objects differ from arrays?

    Objects can include methods (functions) as well as data, whereas arrays can only contain data. Technically, in JavaScript, arrays are an object as well.

4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

    When an object property name is held in a variable, then you can't use dot notation to access the value.

5. Evaluate the code below. What does the term this refer to and what is the advantage to using this?

    `this` is the keyword that refers to the current object the code is being written inside, in this case `dog`.

    ```javascript
    const dog = {
        name: 'Spot',
        age: 2,
        color: 'white with black spots',
        humanAge: function (){
            console.log(`${this.name} is ${this.age*7} in human years`);
        }
    }
    ```

[Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

1. What is the DOM?

    The **Document Object Model (DOM)** is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

2. Briefly describe the relationship between the DOM and JavaScript.

    Since the DOM is an object-oriented representation of a web page, it can be modified with JavaScript (or any programming language set up to use it).

## Things I want to know more about

1. Is the constructor syntax language dependent, or is it commonly set as `new Whatever()`?
