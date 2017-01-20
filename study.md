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
The event loop handles the movement of callbacks from the callback queue into the stack, and prioritizes browser rendering over the callback queue where applicable.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync operations are independent operations that are run in parallel.

Async is a method which simulates having multiple threads in order to avoid blocking the event loop by filling the stack with many slow processes.
When the slow processes sent out are done, they return a callback function to be executed by the stack.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The principal advantage is that by keeping the stack clear of slow events, the browser can render much closer to 60fps.

Disadvantages include the fact that you cannot be certain when an async callback will be run, due to the nature of the event loop, and the fact that handling a large number of async callbacks can be difficult to read and implement for the developer.
```
