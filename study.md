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

## Event Loop

In your own words, describe the event loop and how it works?

```md
  The event loop is the means by which asynchronous functions get passed into
  the call stack from the queue.  If the event loop can see the call stack is
  empty, it add the code in the first position of the task queue to the stack.
```

In your own words, describe the difference between sync and async:

```md
 Sync only executes one operation at a time in in a specific order.  Async
 functions are first sent to a web api before being sent to the call queue, and
 are processed concurrently to functions on the callback stack.
```

What are some benefits and disadvantages of async?

```md
 Benefits are running multiple processes at once and fewer hold ups.  It allows
 you to send slower code to the api and leave just faster processes on the stack.
 It also allows for the render of the page to happen more continuously and not
 be blocked by a slow process.  Disadvantages include being expensive from a
 memory stand-point.
```
