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
The event loop is a browser processing tool for executing queued events passed to it from a webAPI handling some process. It works by passing the wueued event back into the stack (a queue list in itself) which then executes the process in the browser.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync refers to the way in which the stack handles processes. In a sync modle, these events are handled in the order in which they are returned if operating on a single string (FIFO). Async is a way in which to process events in a dispursed manner, outsourcing the process to another location in order to proceed with the next stack item.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Benefits: allows for speedier runtime environments and more responsive UIs.
disadvantages: Things you send to be processed may not be returned in the order in which you would like them to be returned and executed.
```
