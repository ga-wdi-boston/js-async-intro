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
The event loop is more like a gate than a loop. The event loop puts pressure
onto the bottom of the stack, and if the stack is empty, the gate is allowed to
open and put the first thing from the task queue onto the stack. Anything can
be passed to the task queue but ideally it is reserve for slower processes so it
doesn't slow down your stack. The combination of the Web APIs and the task queue
and the event "loop" is what makes an actual side chain loop.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronus functions are called and compiled immediately, where asynchronus
functions are called  but not compiled immediately, they are "put on hold" so to
speak, so that the faster functions can be compiles first.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async is great for slower functions, since they can be "put on hold" meaning
they wont slow down the browsers speed waiting for a response. Instead, the
sync functions can flow normally until the async functions are called back!
However issues can arise when "callback hell" is created from flooding the
task queue with slow async functions. The task queue will be taking functions
faster than it is pushing them to the stack, creating a big backup in the
browser. 
```
