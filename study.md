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
The event loop monitors the stack and task queue and invokes the callbacks in the queue/moves the callbacks to the stack when the stack is empty.

Source: referenced the required readings and videos
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous means one request can be handled at a time and cannot move on to the next request until the current request is complete. Asynchronous means a request can begin and the program can move on to another request before the initial request is complete.

Source: referenced the required readings and videos
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages: program doesn't have to wait for request to complete before moving to another request, program can process many requests, parallel threads,creates a more responsive user experience
Disdvantages: time sensitive processes may not be ideal for async processes, callbacks may get backed up in the queue, "callback hell" (nested callback functions)

Source: referenced the required readings and videos, http://stackoverflow.com/questions/25098066/what-is-callback-hell-and-how-and-why-rx-solves-it,
