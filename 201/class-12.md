# Reflections

Charts! Working with data and how to communicate it is pretty important in my job, and charts are a critical tool for that communication. This is an interesting way to do it. Drawing on a canvas as a performative thing versus having all the data be in the DOM seems like a cool optimization.

## Reading

[JavaScript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)

1. What does the `<canvas>` allow a developer to acheive?

    It allows the developer to draw 2D graphics using JavaScript on an HTML element

2. What is the importance of the closing `</canvas>` tag?

    Unlike the `<img>` element, The `<canvas>` element requires the closing tag `</canvas>`. Any content between the opening and closing tags is fallback content that will display only if the browser doesn’t support the `<canvas>` element.

3. Explain what the getContext() method does.

    The `getContext()` method returns a render context object, whatever that means.

[Chart.js Documentation](https://www.chartjs.org/docs/latest/)

1. What is Chart.js and how it can be brought into your project?

    Chart.js allows you to create charts in your webpage. After attaching the script you can use

    ```JavaScript
    import Chart from 'chart.js/auto';
    ```

    This is an example for if you don't care about bundle size.

2. List 3 different Chart types you can create using Chart.js.

    Bar chart, pie chart, line chart

[Easily Create Stunning Animated Charts with Chart.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

1. What are some advantages to displaying data via a chart over a table?

    They're often more digestible and more meaningful when dealing with large sets of data.

2. How could Chart.js aid your previously created applications visually?

    For salmon cookies, the tables could've been charted to see at a glance a comparative analysis of the performance of the different stores

## Things I want to know more about

1. What the heck is a render context object?
2. What is tree-shaking support?
