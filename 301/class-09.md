# Reading

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming?

    Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

2. What is a pure function and how do we know if something is a pure function?

    - It returns the same result if given the same arguments (it is also referred as deterministic)
    - It does not cause any observable side effects

3. What are the benefits of a pure function?

    The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts

4. What is immutability?

    When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

5. What is Referential transparency?

    Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?

    A software component or part of a program that contains related functionality in a separate file. Modules are used in a larger application with importing and exporting.

2. What does the word ‘require’ do?

    Imports a module

3. How do we bring another module into the file the we are working in?

    Require that other module

4. What do we have to do to make a module available?

    `module.exports`

## Things I want to know more about

1. Why are we using `require` vs `import`? According to some hot take on the internet, `import` is the more modern and flexible syntax which will eventually replace `requre` (except in Node.js). See [this](https://stackoverflow.com/questions/31354559/using-node-js-require-vs-es6-import-export)
2. Was I the only one who couldn't see any of the images in that medium.com article?? Made it a very limited read.
