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
The event loop listens for processing passed off to APIs to return their event,
and adds them back to the stack to run.
```

In your own words, describe the difference between sync and async:

```md
Sync requires the current processing to finish before moving on to the next,
blocking all other code from running.

Async allows the current processing to be moved off of the stack until it
returns its result, allowing other code to run.

In addition to the readings, I ready the Wikipedia page for Asynchronous I/O.

```

What are some benefits and disadvantages of async?

```md
Async allows applications to run faster by not stopping to wait for each process
to finish before working on something else.

The downside to async is that you can't guarantee the order Javascript files
are executed in. This means that if multiple scripts rely on eachother, and they
run out of order, your program may not do what you expect it too or just not work
at all.


```
