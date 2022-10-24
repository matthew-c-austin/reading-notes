# Reflections

This reading is focused on hyperlinks for HTML, normal flow and positioning for CSS, and functions for JavaScript. A few things to take more time learning is the syntactic sugar for arrow functions and function expressions, as well as understanding z-index in CSS.

I'm excited to do pair programming to see how it helps my learning and growth.

## [Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

[Creating Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)

1. To create a basic link, we wrap text or other content inside what element?

    An anchor `<a>` element.

2. The `href` attribute contains what information?

    The web address of the target hypertext reference.

3. What are some ways we can ensure links on our pages are accessible to all readers?

    - Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
    - Don't say "link" or "links to" in the link text — it's just noise. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
    - Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
    - Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here".

## [Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)

[CSS Layout: Normal Flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

[CSS Layout: Positioning](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

1. What is meant by “normal flow”?

    Normal flow is the way that webpage elements lay themselves out if you haven't changed their layout, i.e. you haven't applied any CSS to change the way they behave.

2. What are a few differences between `block-level` and `inline` elements?

    By default, a `block-level` element's content fills the available inline space of the parent element containing it and grows along the block dimension to accommodate its content. The size of `inline` elements is just the size of their content. You can't set width or height on inline elements — they just sit inside the content of block level elements.

3. ___ positioning is the default for every html element.

    Static

4. Name a few advantages to using absolute positioning on an element.

    An absolutely positioned element no longer exists in the normal document flow. Instead, it sits on its own layer separate from everything else. We can create isolated UI features that don't interfere with the layout of other elements on the page (popup info boxes, control menus, rollover panels, UI features that can be dragged and dropped anywhere, etc...)

5. What is a key difference between fixed positioning and absolute positioning

    Whereas absolute positioning fixes an element in place relative to its nearest positioned ancestor (the initial containing block if there isn't one), **fixed positioning** *usually* fixes an element in place relative to the visible portion of the viewport. This means that you can create useful UI items that are fixed in place, like persistent navigation menus that are always visible no matter how much the page scrolls.

## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

[Functions - Reusable Blocks of Code](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Functions)

1. Describe the difference between a function delcaration and a function invocation?

    Function declaration is defining a function (its name, input arguments, return values, etc), whereas a function invocation/call/run/execution is actually running the function. Note: functions are hoisted in JavaScript, so you can call it above its definition.

2. What is the difference between a parameter and an argument?

   No difference, they are equivalent. Arguments/properties/parameters are synonymous.

## Miscellaneous

[65 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

1. Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.

    Greater efficiency is interesting to me. Not that it is faster in the first place, but in the long run it produces less technical debt, fewer errors, and just generally higher quality code. It is another avenue to learn from others and increase my skills by colloborating with another dev with a different style or approach.

    And of course being able to say I've done pair programming is a leg up in an interview at a company that engages in the practice.

## Things I want to know more about

1. Do any of the big FAANG companies regularly do pair programming?
2. Is the alternate box model more common or recommended vs the standard model? This goes back to the last reading, but it's been on my mind.
