# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.

```md
The event loop invokes the callback and the callback functions are passed as arguments until the I/Os are complete and the return value is available, which then gives an event.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
synchronous tasks will take precendent until the task at hand has completed, then the next task can be started. Each step has to be completed one after the other but another step cannot start until the first has finished. synchronous functions block the even loop so they should be avoided.
asynchronous tasks can start and then be put aside while other tasks are started and completed. These should be used since they are more efficient.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
advantages:
clearer and cleaner


disadvantages:
errors are easier to miss
callback hell => messy code
functions that are asynchronous don't return right away
```
