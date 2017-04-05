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
The event loop looks at the stack and callback queue. If the stack is empty, it takes the first thing on the callback queue and pushes it onto the stack.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
sync: when things run one at a time.

async: when code is executed out of order; in javascript, it's essentially referring to code that puts things in the queue. You could have the setTimeOut to 0, which puts it in the queue - which then actually allows for things to run concurrently instead of blocking the stack.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantage: since it allows for code to run concurrently, things happen more quickly when using async. Without async, the browser can get stuck.
Disadvantages: it can be very hard to debug when the code is more complex. You also can't return it or error handle it.
```
