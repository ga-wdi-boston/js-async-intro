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
Event loops work with a message queue to utilize asynchronously-fired callbacks, which in turn allows for multiple operations to be handled while waiting for an external event (e.g. a click). An event loop works by invoking a callback function once a return value from the respective I/O call is available.

Additional resources:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop
http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/
```

In your own words, describe the difference between sync and async:

```md
Sync is where a program must stop while it waits for indiviual I/O operations to finish (e.g. response-request model). Async allows multiple I/O calls to be performed without stopping the entire process. In async, the calls run independently of one another.
```

What are some benefits and disadvantages of async?

```md
Advantages to using async include making an application run more efficiently and being simple enough for JS programmers to understand and use. However, async can only process one request at a time (a.k.a. single-threaded). A disadvantage to this is that if the program hits a very time-consuming function or an infinite loop, the entire process can still get blocked.
```
