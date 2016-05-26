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
The event loop is the process through which code is executed.  First, a function is initialized and will either go to the stack for processing or it will go to the web api for processing.  Once processing is completed, the messages from the code will go to the message queue to be processed.  Messages can only be processed once at a time, so the queue can contain many messages that are waiting to be processed.
```

In your own words, describe the difference between sync and async:

```md
With sync, a process must be completed before another task can be run, so all processes are halted until the current process is finished.  With async, processes can be run at the same time and do not need to wait for one another to be completed before the next process is begun.
```

What are some benefits and disadvantages of async?

```md
Some benefits of async are that numerous function calls can be run at one time.  So, you don't have to wait for one process to end before another begins.  A disadvantage can be that you can't control the order in which code get executed.

https://www.nccgroup.trust/uk/about-us/newsroom-and-events/blogs/2015/july/what-are-the-benefits-and-drawbacks-of-loading-javascript-asynchronously/

```
