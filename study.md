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
Javascript is 'single threaded', so only one task at a time can be executed.
The event loop checks functions in the runtime stack and in the queue and pushes events from the queue to the stack when the stack is empty.

I used: https://www.youtube.com/watch?v=vMfg0xGjcOI
https://blog.risingstack.com/node-hero-async-programming-in-node-js/
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous tasks are events that are blocking. When events need to be called in strict order, they are synchornous.
Async is when events are not blocking other events from happening. If an event takes time to complete (like a timer function), other events can happen in the mean time.

I used :
https://blog.risingstack.com/node-hero-async-programming-in-node-js/
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/

```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async allows functions to be executed in the fastest and most efficient way possible in many circumstances because they don't allow any time to be wasted.
Using them too liberally can make code look complicated and hard to decipher. We can have something called callback hell if too many functions are nested within each other.

I used: https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```
