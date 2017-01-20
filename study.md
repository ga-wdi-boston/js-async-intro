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
An event loop pulls the first item in the task queue and moves it to the stack when the stack is empty.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync is step by step, one line at at time. Async will allow things to happen out of order or at the same time so you don't know when they will finish.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
+ Lets things happen out of order
+ Doesn't block the browser
- Don't know when things will execute
```
