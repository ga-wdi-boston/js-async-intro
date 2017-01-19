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
The event loop is how javascript decides what to do next. Since it can only do one thing at a time, it sometimes puts off longer tasks until the quicker or more urgent ones are done. Or until it gets a response from another computer.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync is when you do one thing at a time, strictly. So for example, if you request info from a server, you then just have to wait until the server responds before you can do anything else. Async is when you can put tasks on the back burner, so like when you request something from a server and while you're waiting for a response, you finish loading a file on your own machine.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async prevents long tasks from blocking the queue, so you can do other stuff while you wait for long tasks to complete. However, it means that those long tasks can build up themselves and you end up in callback hell, with way too many things you're waiting to do.
```
