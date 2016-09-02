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
The event loop is a way to asynchronously call functions contained in the same thread.
If a function is moved out of the stack and in to the queue, it will not be run until the stack is free of functions to run. Once the stack has cleared, the que will begin to populate the stack again.
(http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/)
(http://altitudelabs.com/blog/what-is-the-javascript-event-loop/)
```

In your own words, describe the difference between sync and async:

```md
Sync is when all functions in a thread are run concurrently.
Asynch is when functions are called out of order from other functions.
Other functions are not dependent on the asynch functions' immediate completion.

(http://rowanmanning.com/posts/javascript-for-beginners-async/)
```

What are some benefits and disadvantages of async?

```md
Asynch allows functions (that would normally take a long time to run) to run without impeding other functions required to have a functioning (ha ha) web app. These asynch functions can 'do their own thing' without slowing or stopping other elements in the browser.

Asynch can cause a mess of recursive callback functions that endlessley trigger.
```
