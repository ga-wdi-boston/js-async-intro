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
Node uses an event loop for scalability, instead of processes or threads. In contrast to other event-driven servers, Node event loop does not need to be called explicitly. Instead callbacks are defined, and the server automatically enters the event loop at the end of the callback definition. Node exits the event loop when there are no further callbacks to be performed.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
synd is doing one thing at a time abd async is doing multiply thins at the same time
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
advantage : run code better and to multitask
disadvantage: callback hell makes problems
```
