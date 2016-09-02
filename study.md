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
  The event loop is the means by which asynchronous functions get passed into
  the call stack from the queue.
```

In your own words, describe the difference between sync and async:

```md
 Sync only executes one operation at a time in in a specific order.  Async can
 send functions into the call stack as soon as they are completed, and slow
 processes won't hold up the entire stack.
```

What are some benefits and disadvantages of async?

```md
 Benefits are running multiple processes at once and fewer hold ups.  Some
 disadvantages include being expensive from a memory stand-point.
```
