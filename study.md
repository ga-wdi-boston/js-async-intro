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
The event loop is a complete looping process through stack and queue. It first runs through all non-blocking I/O and throw those callback functions to web api to respond. But at the same time stack will continue to run through rest of the non-blocking I/O. After web api responds for requests, it throws messages to queue to store and give back to stack. Since JavaScript is single-threaded, functions can only be processed once at a time, so the queue can store many messages that are waiting for stack to be processed.
Reference: http://altitudelabs.com/blog/what-is-the-javascript-event-loop/
```

In your own words, describe the difference between sync and async:

```md
sync means functions should run one after another, and next function always need to wait for previous function finished processing;
async means several functions can be run at the same time, and they won't need to wait for previous function finished processing;
```

What are some benefits and disadvantages of async?

```md
The most beneficial part of async is that it can process several functions at the same time, which is essential for handling heavy traffics; But this can be a problem at sometimes that you want to control processing order of functions.
```
