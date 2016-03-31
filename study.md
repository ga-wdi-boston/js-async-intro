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

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop searches for tasks in a queue to execute from callback functions
read earlier, going through the single thread processing of JS.  It takes these
events and puts them on the Call Stack to have their code executed.
```

In your own words, describe the difference between sync and async:

```md
Synchronous functions must complete in their entirety before the single thread
processing of JS can move on through the code, while asynchronous functions are
read, and then put into the Callback queue to be executed at a later time.  It is
important to use async for time/processing intensive functions, so that a user can
continue to smoothly interact with the browser.  Sync functions will freeze their
browser until the functions are complete.
```

What are some benefits and disadvantages of async?

```md
Async allows for a smooth and fluid UI/broswer expereience for users, however it
can be disadvantageous if other functions depend on an async function's output,
since the function calling the async function will not be able to complete since
output is produced later on or at the end of all other CallStack operations.
```
