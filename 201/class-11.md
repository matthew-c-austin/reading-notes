# Reflections

This topic was a bit more in depth in audio and video content for HTML, a look at grid based layouts in CSS, and some responsive images info. The responsive images and the idea of responsive and dynamic page design is something that I've been wanting to get an introduction to since seeing it in basically every real-life example of a webpage.

## Reading

[Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.

    Proprietary plugin-based tech like Flash and Silverlight dominated the web back in the day. Their accessibility and security issues were problematic, and nowadays you can use APIs from JavaScript or OVPs like YouTube and Soundcloud.

2. Describe the use of the `src` and `controls` attributes in the `<video>` element.

    It works the exact same way as with an image. It points to the source path to the video you want to embed.

3. Why is it important to have `fallback content` inside the `<video>` element?

    In case the browser or software being used doesn't support the source codec for the video.

4. Write a very short story where `<audio>` and `<video>` are characters.

    `<video>` was the loud friend. `<audio>` was quiet. This was backwards, but it's true. `<audio>` had no `width` or `height`, no poster attribute. It was only heard, not seen. `<video>` demands so much more.

[A Complete Guide To Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

1. How does Grid layout differ from Flex?

    Grid is two-dimensional flow, whereas flexbox is one-dimensional.

2. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

    - Grid container: is the element on which `display: grid` is applied. It's the direct parent of all the grid items.
    - Grid item: The children (i.e. *direct* descendants) of the grid container.
    - Grid lin: The dividing lines that make up the structure of the grid. They can either be vertical "column grid lines" or horizontal "row grid lines", and they reside on either side of a row or columne.

[Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

1. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

    Displaying a large image on a screen smaller than it was meant for wastes bandwidth

2. Define the following `<img>` attributes `srcset` and `sizes`. Write an example of how they are used.

    `srcset` defines the set of images we will allow the browser to choose between, and what size each image is.

3. How is `srcset` more helpful for responsive images than CSS or JavaScript?

    Because of the order of loading a web page. If the purpose is to reduce bandwidth, the images are loaded before the main parser has started to load and interpret the page's CSS and JS. Handling it in the HTML allows for responsive image design that actually saves bandwidth.

## Things I want to know more about

1. I wasn't aware at all that MP3 and other formats of codecs were patent protected and that you need to pay fees to host them. I just want to learn more about this in general, and what codecs to use.
2. Why do you only use media in art direciton scenarios?
