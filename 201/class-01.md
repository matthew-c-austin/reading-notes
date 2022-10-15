# Reflections

This reading assignment lays the foundation for the rest of the class. It was a good reminder of what was done in 102, and it's a primer of new topics that we'll probably cover early into the 201 course (async/defer/intricacies of how the web works).

## [Getting Started](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)

### Links

[How the Web Works](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)

[Website Design and Process](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like)

[JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)

### Questions

**Q:** Compose a short poem describing how HTTP sends data between computers.

HTTP. How does it serve me?

It is the lingua franca of our wide world webbed. Let's sail that high sea.

Chart a course over the horizon, with your trusty DNS map to guide you to the shining Server city.

You arrive at Port 80, your ship the *Request* is held at the dock, a pity.

Find the Port Master. He shouts above the din what dialect he speaks in,

"HTTP/1.1"

You tell him what you wish to take home with you.

"200 OK". It's done.

The *Request*, laden with packets heads home to a familiar shore.

That is, until the *Request* wants some more.

**Q:** Describe how HTML, CSS, and JS files are “parsed” in the browser

**A:**

- The browser first parses the HMTL file, which let's it recognize any `<link>` element references to external CSS stylesheets and any `<script>` elements.
- As the browser parses the HTML, it sends back requests for any CSS files and any JavaScript files found in those elements, then it parses the CSS and JavaScript.
- The browser generates an in-memory **DOM** tree from the parsed HTML, then it generates an in-memory **CSSOM** structures from the parsed CSS, and then it compiles and executes the parsed JavaScript.
- As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a page is painted onto the screen which the user can begin to interact with.

**Q:** How can you find images to add to a Website?

You can go to google and save an image from the image search or copy the web address for the image. Note: most stuff on the web is copyrighted. You can use Google's license filter.

Click on the Tools button, then on the resulting Usage rights option that appears below. You should choose the option Creative Commons licenses.

**Q:** How do you create a `String` vs a `Number` in JavaScript?

**A:** A string has quotes around it such as

```Javascript
let myVariable = 'Bob';
```

Numbers don't have any quotes around them, and obviously they need to be numeric.

```Javascript
let myVariable = 10;
```

**Q:** What is a `Variable` and why are they important in JavaScript?

**A:** Variables are containers that store values. You can declare, assign initial values, change their values, their data types, and more.They are necessary to do anything interesting in programming. They allow dynamic actions within your code.

## [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)

### Links

[Getting Started with HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

[HTML Document Structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)

[Medadata in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)

### Questions

**Q:** What is an HTML attribute?

**A:** An **attribute** contains additional information about an element that won't appear in the content.

**Q:** Describe the Anatomy of an HTML element.

**A:**

- **The opening tag**: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.
- **The content**: This is the content of the element. In this example, it is the paragraph text.
- **The closing tag**: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

The element is the opening tag, followed by content, followed by the closing tag.

**Q:** What is the Difference between `<article>` and `<section>` element tags?

**A:** Whereas `<section>` is for grouping distinct sections of content or functionality, `<article>` is for containing related individual standalone pieces of content, such as individual blog posts, videos, images or news items. Think of it this way - if you have a number of items of content, each of which would be suitable for reading on their own, and would make sense to syndicate as separate items in an RSS feed, then `<article>` is suitable for marking them up.

[Reference](https://stackoverflow.com/questions/7549561/section-vs-article-html5)

**Q:** What Elements does a “typical” website include?

**A:** Typical websites will include the following elements:

1. The `<html>` element. This element wraps all the content on the page. It is sometimes known as the root element.
2. A `<head>` which does not show up on the page. This element acts as a container for everything you want to include on the HTML page, that isn't the content the page will show to viewers.
3. The `<meta>` element. This element represents metadata that cannot be represented by other HTML meta-related elements
4. The `<title>` element. This sets the title of the page, which is the title that appears in the browser tab the page is loaded in.
5. The `<body>` element. This contains all the content that displays on the page, including text, images, videos, games, playable audio tracks, or whatever else.
6. A `<header>` element. Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.
7. A navigation bar `<nav>` element.
8. Main content: `<main>`, with various content subsections represented by `<article>`, `<section>`, and `<div>` elements.
9. Sidebar: `<aside>`; often placed inside `<main>`. Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.
10. A footer `<footer>` element. A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself.

**Q:** How does metadata influence Search Engine Optimization?

**A:** Search engines like Google don't "read" the content of your website. They index by seeking out info from defined metadata fields (things like search engine title, description, author, keywords, copyright, etc...)

**Q:** How is the `<meta>` HTML tag used when specifying metadata?

**A:** Within the `<meta>` tag you can add all kinds of other elements, most of which contain `name` and `content` attributes. There's tags for adding icons in favorites or homescreens. There's proprietary tags for displaying links on sites like Facebook and Twitter. Many weren't covered in the primer linked above.

## Miscellaneous

### Links

[How to start to design a Website](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)

[Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

[What is JavaScript?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

### Questions

**Q:** What is the first step to designing a Website?

**A:** Planning! A website should have some functionality in mind before you begin. What do you want to accomplish? Project ideation is a necessary first step. Things that should be answered:

1. What is your website about?
2. What information are you presenting on the subject?
3. What does your website look like?

**Q:** What is the most important question to answer when designing a Website?

**A:** What exactly do I want to accomplish?

**Q:** Why should you use an `<h1>` element over a `<span>` element to display a top level heading?

**A:** Using a semantic tag gives context to the content within the tag. It is the default semantic tag for that purpose, which gives it the benefits listed in the answer to the following question.

**Q:** What are the benefits of using semantic tags in our HTML?

**A:**

- Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
- Screen readers can use it as a signpost to help visually impaired users navigate a page
- Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
- Suggests to the developer the type of data that will be populated
Semantic naming mirrors proper custom element/component naming

**Q:** Describe 2 things that require JavaScript in the Browser?

**A:**

1. Running code in response to events occuring on a web pag, such as a button click or a mouse-over.
2. Manipulating the HTML and CSS of a web page to dynamically apply new styles, popups, etc...

**Q:** How can you add JavaScript to an HTML document?

**A:** You can either do internal JavaScript using a `<script>` tag, or, more commonly, use an external JavaScript file. This allows the HTML to look cleaner and easier to read, and it allows the JavaScript code to be reusable across multiple HTML files.

## Things I want to know more about

1. How does your computer know how long to hold the DOM and CSSOM in memory? Is this something the browser handles (garbage collection after a tab close?)
2. Is it more common to use async or defer when writing JavaScript code? Or is the answer "it depends"?
3. Is  `<!DOCTYPE html>` an element?
4. Is there a typical metadata template used in most cases, or are they built from the ground up for each page?
