# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

These studies focus on the differences between Asynchronous Code, and
Synchronous Code. For the most part, you can think of the differences as the
following. However, the readings will go into much more detail on the
differences and patterns of each.

Synchronous Code - operations the occur sequentially: ask db for data; wait; db gives data; do something with data.

Asynchronous - operations that may start in a certain sequence and may end in any permutation of that sequence while unrelated stuff happens in between.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.

```md
An event loop is a queue of callback functions.  When an async function is executed, the callback function is pushed into the queue.  Event loops are responsible for invoking callbacks.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Async tasks can be started and put aside until later where as sync tasks run until its completed.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Disadvantage: Async functions usually use callbacks which could result in many nested callbacks.  This can make the code look messy and hard to read.

Advantage: Async functions can run independently, unlike sync functions it doesn't have to finish one task before starting another one.   
```
