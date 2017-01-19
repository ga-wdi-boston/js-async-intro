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
The event loop is a process that looks at the task queue, where webapis would have
put callback functions into once their async functions complete, and if the
JS callstack is clear, pushes those callback functions onto the callstack. It is
worth noting that JavaScript is a single-threaded language, meaning it is
synchronous and can only run things in order, and not have multiple callstacks
running code concurrently (it only has one callstack). The asynchronous
functionality is provided by WebAPIs and not by the V8 (JS) runtime itself. 
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync means that code is executed in the same order (exactly) that the code is
put on to the stack. With synchronous items you can easily predict in what
order they will be executed. However, async means that code may not be executed
in a fully predictable, ordered manner. Asynchronous items can executed at some
later step (usually after some conditions are met, such as setTimeout waiting
for a certain amount of time to pass).
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
One of the main benefits to async is that you can execute other code and not
halt your stack calls while waiting for a particular async block to execute.
A disadvantage is that sometimes you can't predict when some code will be
executed by the callstack using async; it will happen at some point in the
future (potentially), you just can't be sure of when.
```
