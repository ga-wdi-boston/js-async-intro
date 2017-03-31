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
The event loop looks at the current stack and callback task queue.  If
the stack is empty it takes the first thing on the callback task queue and
pushes it onto the stack for it to be executed.

References:
[What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync events can only be run one at a time (single-threaded).  A sync event needs to be completed before another sync event can begin.

Several async events can be run in parallel using non-blocking I/O and
an event loop.

References:
Text in this study above

https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Several synchronous calls will lock up the browser over time and
asynchronous calls will not lock up the browser as these calls are
done concurrently or in parallel.

A disacdvantage of async programming is that it adds more complexity
to the developer's JavaScript code.

References:
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/

https://www.quora.com/What-are-the-disadvantages-of-asynchronous-callback-mechanism-on-the-server-side
```
