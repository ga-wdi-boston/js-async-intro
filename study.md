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
The event loop checks both the stack and the task queue and whenever the stack is empty, it pushes the task from the front of the queue to the stack. This means that asynchronous events will only occur when your code has finished running.
```

In your own words, describe the difference between sync and async:

```md
Sync means that events happen in order, one after another in the order they were called. Async means that events can be processed elsewhere and occur once completed, not necessarily in the order in which they were called.
```

What are some benefits and disadvantages of async?

```md
An advantage is that time consuming processing doesn't have to lock up the browser until it's complete. A disadvantage is that it's more difficult to determine when various events will be complete and you can use the results of those events.
```
