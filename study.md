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
The event loop waits until the stack is clear and push's a task from the que onto it.
The tasks on the que are responses to requests we made to an api.

https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.


```md
Synchronous code will block the stack, performing a slow operation, preventing any javscript or operations in the broswer from running until it is done.

Asynchronous doesnt block the stack with slow operations. It would make a request to an API,
set up a listener and move on to the next piece of javascript. When the API responds the listener
it calls a function which gets pushed to the stack by the event loop. This leaves space for other things
to happen while the server gathers the information we requested
https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages:

We get to perform multiple operations(threads) at once by communicating with an API. This prevents the
browser from being sluggish, maintaining a fluid user experience

Disadvantages:

It could slow be slower if we send small tasks to an API to be processed. Tasks that would be quicker to
perform sequentially without having to wait for a server to respond.
https://www.quora.com/What-are-the-disadvantages-of-asynchronous-callback-mechanism-on-the-server-side
```
