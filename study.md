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

The event loop describes how and when async callback functions finally get
executed.  The callback function is put on a queue.  When the async function
is completed, the callback function is then executed.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync - everything happens linearly.  Async - the task is begun but other stuff happens while it is running.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
advantages: the entire program is not halted until a (possibly long) call is finished.
disadvantages:  the program is non-linear and is harder to write, understand, and debug.
```
