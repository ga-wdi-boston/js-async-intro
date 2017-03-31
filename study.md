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
The event loop is a holding place for callback functions that have been returned by their enclosing function, but are waiting to execute on the stack. The stack must clear before the the callback is executed.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchoronous refers to code that executes from top to bottom, waiting for completion of one step before proceeding to the next.

Asynchronous refers to the fact that browsers hand off certain functions (passing a callback) to web APIs to process in the background, executing the callback after the background process completes (via the event loop). This can result in your code not executing top to bottom as it is written, which is what asyn refers to.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage is that the stack isn't bogged down by slow, blocking functions (like long while loops, or file download).

Disadvantage is that you can't always know in which order your code will execute, which could make your website behave strangely and be hard to debug. 
```
