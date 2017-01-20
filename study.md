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
The event loop is a mechanism in the browser for javaScript functions. When functions get called, their requests normally slow down the performance of a web application, but this set up helps to manage it in the way that releases them one by one. The path is as followed - from the function's requests to a call stack where they get in the first place then they go to web api server (heap) and third place where they get stored is the event queue. When the call stack gets available space again then the function which is already in this time a message gets to be processed back to call stack. All for smoother quicker performance while using setTimeout functions.
```
https://developer.mozilla.org/en-US/docs/Glossary/Call_stack

and your video
https://www.youtube.com/watch?v=8aGhZQkoFbQ

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
A good question and I looked asynchronous up. Synchronous means that one event start and next event starts after the first one finishes. Or in terms of function calling - when I call a function I have to wait until the previous task is finished.

Asynchronicity - when I call the function it starts without waiting to finish current process - thread.

http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages - it's good to have a program  and split it of into another threads -  run times to process more tasks in the same time. Plus these threads can pass messages to each other.
your link
https://www.youtube.com/watch?v=vMfg0xGjcOI

Disadvantages - time lost waiting for a response and complexity


```
