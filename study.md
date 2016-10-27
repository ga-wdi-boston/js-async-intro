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
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until section on fibers)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
Javascript engine executes the functions available in the call stack. If there
is any callback function, it is first loaded into the event table, and when it
is ready to be executed, it is moved to the event queue.
If teh callstack is empty, the callback functions in event queue will be
executed next. This process of listening to all these tables and queues are
handled by the event loop.
```

In your own words, describe the difference between sync and async:

```md
Sync is a sequential flow of execution of functions.
Async functions are not a blocking code, which means it gets executed later.
```

What are some benefits and disadvantages of async?

```md
Benefits:
Since the callback functions are not executed until thye call stack is free, it
is not a blocking code.
Disadvantage :
The order in which asynchronous functions are executed cannot be guaranteed.
```
