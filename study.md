# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until section on fibers)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop organizes a queue of asynchronous callback functions. In essence, the event loop waits until the call stack is empty, then pushes one function from the queue to the call stack so it can run/be called.
```

In your own words, describe the difference between sync and async:

```md
Sync, or synchronous, carries tasks to completion and waiting for each call to process before moving on to the next one. On the other hand, async or asynchronous sort of allows multiple things to happen at once, as asynchronous task can be initiated and then put aside until a later date while getting started on the next task.
```

What are some benefits and disadvantages of async?

```md
Pros:

High-priority functions can be prioritized as slow/low-priority functions can be kept from running until the higher-priority ones have been executed

Multiple threads of code can be run somewhat simultaneously. Although there is still
only one stack, the event loop lets us keep a queue of function calls that are separate from the browser's running stack.


Cons:

Async is more complex since an embedded callback function is needed to delay a
function's execution, meaning that our code could be harder to read/debug if we have to write several callback functions at a time.
```
