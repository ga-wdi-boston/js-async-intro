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
The event loop is essentially javascript's way of running code quickly and
efficiently. The use of callbacks in javascript allow for asynchronicity in
processing in the browser. Code with shorter runtime (that does not require waiting for another function/information) to process, gets placed in the stack and is run. Code that takes longer can begin to be processed at the same time while it ways for other things to be processed, so it is placed in a queue until the stack clears. When the stack clears and the necessary information has been processed for the callback, that function can move into the stack to finish processing. The event loop is responsible for moving this code from the queue to the stack.

source: video & https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop

```

In your own words, describe the difference between sync and async:

```md
Synchronous means that pieces of code can only be processed one at a time.
Async means that multiple pieces of code can be processed at once.

source: class notes.
```

What are some benefits and disadvantages of async?

```md
Asynch is beneficial because it provides more seamless, clean, reuseable code, and may create less work for the developer. However, it can be difficult to find errors when they occur because there are usually functions embedded within functions and other
complex code that is written. Sometimes, writing asynchronous code in itself can become complex and difficult to read.

notes: class and this blog: http://www.html5rocks.com/en/tutorials/async/deferred/
```
