# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop is responsible for the order that each callback function gets processed. It starts the functions and wont move on to the next one until the current one is done.
```

In your own words, describe the difference between sync and async:

```md
When you are talking about sync, you are saying that youre waiting for the first step/function to execute before you move on. For an async situation, you can start doing other things before the step/function is done running.
```

What are some benefits and disadvantages of async?

```md
It is really important to make sure things are in order when youre working with functions. One example could be to want a list to be displayed and then organized alphabetically, you could then have a problem with someones connection loading the page slow and because you tried to organize the page in alphabetical order before it was displayed maybe it wouldn't load at all.
```
