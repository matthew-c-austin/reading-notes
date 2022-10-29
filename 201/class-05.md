# Reflections

This reading is focused on images in HTML and color and fonts for CSS. There is a focus on accessibility for all topics, and it should be front of mind when making decisions in website layout as part of achieving a delightful user experience.

## [Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

[Using Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

[Common Image Types and Choosing Image Formats](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types)

1. What is a real world use case for the `alt` attribute being used in a website?

    The user is visually impaired, and is using a screen reader to read the web out to them. In fact, having alt text available to describe images is useful to most users.

2. How can you improve accessibility of images in an HTML document?

    Including `alt` attributes in every image (that's not decorative). Don't write redundant `alt` text, and don't put text into images.

3. Provide an example of when the `figure` element would be useful in an HTML document.

    Usually a `<figure>` is an image, illustration, diagram, code snippet, etc., that is referenced in the main flow of a document, but that can be moved to another part of the document or to an appendix without affecting the main flow.

4. Describe the difference between a `gif` image and an `svg` image, pretend you are explaining to an elder in your community.

    A `gif` is an audioless animation or image that is good for simple use cases where quality isn't a big concern. An `svg` let's you maintain accurate pictures at different sizes for different screens, for instance. It's mostly used for logos/icons/diagrams/interface elements.

5. What image type would you use to display a screenshot on your website and why?

    PNG or lossless WebP, JPEG if compression artifacts aren't a concern.

## [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

[Using Color in CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color)

[Styling HTML Text Elements](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

1. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

    The `color` property is for foreground color of any element, whatever is in front (take text for example). `background-color` is a property that is everything behind that text.

2. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

    Coming up with right colors is tricky, but the first step would be to choose a base color. Something that is naturally associated with the topic of the blog.

    When designing the rest of your palette, consider color theory resources and accessibility for the visually impaired.

3. What should you consider when choosing fonts for an HTML document?

    Whether the choice of font is "web safe" i.e. widely available on all types of operating systems. You can apply a "font stack", a list of fonts the browser attempts to use, in order. Generally, a generic font should be put at the end.

    ```CSS
    p {
    font-family: "Trebuchet MS", Verdana, sans-serif;
    }
    ```

4. What do `font-size`, `font-weight`, and `font-style` do to HTML text elements?

    - Font size (set with the `font-size` property) can take values measured in `px`, `em`s, and `rem`s to size the text.
    - `font-style`: Used to turn italic text on or off.
    -`font-weight`: Sets how bold the text is. This has many values available in case you have many font variants available (such as *-light*, *-normal*, *-bold*, *-extrabold*, *-black*, etc.), but realistically you'll rarely use any of them except for `normal` and `bold`

5. Describe two ways you could add spacing around the characters displayed in an `h1` element

    The `letter-spacing` and `word-spacing` properties allow you to set the spacing between letters and words in your text.

## Things I want to know more about

1. Having never seen .webp in any image creation (even downloading from the internet), is this a newer format, and should we be using it as a default?
