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
The event loop handles queueing asynchronous callbacks onto the stack whenever
the stack is free to process another function.
```

In your own words, describe the difference between sync and async:

```md
a sync function process the code one line at a time, and doesn't move on until 
it has finished what its currently processing.  Async code can defer certain
functions, like callbacks, and continue processing the code until its done, then
the event loop feeds the callbacks that were deferred back into the stack.
```

What are some benefits and disadvantages of async?

```md
Instead of having to wait for a callback that might take a while to process to
finish, it can push the longer callback to the queue and continue to process the code,
returning to the callback once its finished its other pending tasks.
```
