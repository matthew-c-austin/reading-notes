# Reflections

This reading focuses on local storage for web applications, and a few reasons why you might use them (such as memoizing/caching state information or long lead time info from an API).

## Reading

[Local Storange and How To Use It On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

1. Why would a developer use local storage for a web application?

    If you want to cache data from the web when it takes a long time to get it, or if you want to store the state of intefaces

2. What information should not be stored in local storage?

    User password data/personal data.

3. Local storage can store what type of data? How would you convert it to that type before storing?

    Strings. You would use `JSON.stringify()` and `JSON.parse()`

## Things I want to know more about

1. Is local storage used consistently and by convention? Or is it generally preferred to use server side storage or some Content Delivery Network?
