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
The event loop is a system which checks the runtime stack and the callback task queue and pushes tasks in the callback queue into the stack once it is empty. 

- https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous tasks refer to tasks that are blocking. The new tasks must wait for previous tasks to complete before executing.

Asynchronous tasks refer to tasks that are non-blocking. If a task takes time to complete, the engine can move on to other tasks and get "called back" when the original task completes.

- https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
- https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async tasks are advantageous because the allow the server to move on to other tasks rather than waiting for an original taks to complete.

They can be a disadvantage because even relatively simple tasks can require many callback functions which can make the code difficult to understand and work with.

- https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```
