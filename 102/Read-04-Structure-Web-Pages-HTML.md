# Structure Web Pages with HTML

## Wireframe and Design

[How To Make Your First Wireframe](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)

### What is a Wireframe?

UX designers used wireframes to define and plan information hierarchy for websites, apps, or products. The process focuses on how the designer or client wants the user to process information on a site, based on the user research already performed by the UX design team.

- It is in plain black and white, without code
- No colors or typeface choices lets you plan without distraction
- A button or call to action should be clear to the user even if it's not brightly colored and flashing.

### Wireframe Examples

Wireframes can be made by hand or with software like [Invision](https://www.invisionapp.com) or [Balsamiq](https://balsamiq.com/). Another free web based app is [wireframe.cc](https://wireframe.cc/).

It's likely to your advantage to start by hand-drawing your wireframes before executing more detailed versions using an online app or software.

### 6 Steps to Make a Wireframe

1. Do your research
2. Prepare your research for quick reference
3. Make sure you have your user flow mapped out
4. Draft, don't draw. Sketch, don't illustrate
5. Add some detail and get testing
6. Start turning your wireframes into prototypes

### How to Make Your Wireframes Good

Three key principles to keep in the forefront of your mind

1. Clarity: Your wireframe needs to answer the questions of what that site page is, what the user can do there, and if it satisfies their needs. Your wireframe is an aid for you to visualize the layout of your site page and ensure that the user’s most important questions are answered and goals are achievable without being distracted by more aesthetic considerations.
2. Confidence: Ease of navigation through your site and clear calls-to-action increase user confidence in your brand. If your site page is unpredictable, or has buttons or boxes in unexpected places user confidence diminishes. A lot of this information can already be organized at the wireframing stage. Using familiar navigational processes and placing buttons in commonly-used and intuitive positions, user confidence will soar–and that’s before you’ve even gotten around to thinking about colors and styles.
3. Simplicity is key: Too much information, copy, or links, can be distracting to the user and will have a detrimental affect on your users’ ability to achieve their goals. You want your users to be able to find their way through your site with as little extra ‘fluff’ as possible, to the elements that map to their most significant goals in a given context.

## Mozilla HTML Basics

[Resource Link](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)

HTML (HyperText Markup Language) is the code that is used to structure a web page and its content. For example, content could be structured within a set of paragraphs, a list of bulleted points, or using images and data tables.

HTML consists of a series of **elements**, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing **tags** can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.

### Anatomy of an HTML Element

![HTML Element](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)

The main parts of our element are as follows:

1. The opening tag: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
2. The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
3. The content: This is the content of the element, which in this case, is just text.
4. The element: The opening tag, the closing tag, and the content together comprise the element.

Elements can also have **attributes**. Attributes contain extra info about the element that are not visible in the actual content. Attributes should have the following:

1. A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
2. The attribute name followed by an equal sign.
3. The attribute value wrapped by opening and closing quotation marks.

You can put elements inside other elements too — this is called **nesting**.

Some elements have no content and are called **empty elements**. An image element is an example. The purpose of a `<img>` element is to embed an image, and thuse has no content to wrap.

### Anatomy of an HTML Document

- `<!DOCTYPE html>` — doctype. It is a required preamble. In the mists of time, when HTML was young (around 1991/92), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML, which could mean automatic error checking and other useful things.
- `<html></html>` — the `<html>` element. This element wraps all the content on the entire page and is sometimes known as the root element. It also includes the lang attribute, setting the primary language of the document.
- `<head></head>` — the `<head>` element. This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like keywords and a page description that you want to appear in search results, CSS to style our content, character set declarations, and more.
- `<meta charset="utf-8">` — This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages. Essentially, it can now handle any textual content you might put on it. There is no reason not to set this and it can help avoid some problems later on.
- `<meta name="viewport" content="width=device-width">` — This viewport element ensures the page renders at the width of viewport, preventing mobile browsers from rendering pages wider than the viewport and then shrinking them down.
- `<title></title>` — the `<title>` element. This sets the title of your page, which is the title that appears in the browser tab the page is loaded in. It is also used to describe the page when you bookmark/favorite it.
- `<body></body>` — the `<body>` element. This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.

## Semantics

[Resource Link](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

In programming, Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", or "what purpose or role does that HTML element have" (rather than "what does it look like?".)

HTML should be coded to represent the data that will be populated and not based on its default presentation styling. Presentation (how it should look), is the sole responsibility of CSS.

## Additional Resources

[Mozilla HTML Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)

[Mozilla HMTL Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)