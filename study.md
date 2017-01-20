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
<!-- The event loop is when there functions are put into a call stack because only one function can be executed at a time. other functions are put into a queue to be executed, as the stack functions are executed the queue loops the ones that havent been called yet to the stack.-->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!-- sync would be things running concurrent with eachother, async means that one thing at a a time runs but while we are waiting for a function to finish we can execute another function.  -->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!-- advantages running things faster and smoother
dis advantages not knowing exactly the order or timing of functions to finish executing-->
```
