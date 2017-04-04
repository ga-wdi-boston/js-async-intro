# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

These studies focus on the differences between Asynchronous Code, and
Synchronous Code. For the most part, you can think of the differences as the
following. However, the readings will go into much more detail on the
differences and patterns of each.

Synchronous Code - operations the occur sequentially: ask db for data; wait; db gives data; do something with data.

Asynchronous - operations that may start in a certain sequence and may end in any permutation of that sequence while unrelated stuff happens in between.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.

```md
When your code runs, the event loop monitors the call stack (a data structure that informs JS where we are in the program) and the task queue. Once JS finishes running tasks in the call stack, the event loop will take the first callback on the task queue and push the task to the call stack so that it can be run. It's important to note that the event loop cannot push the callback onto the stack until the call stack is clear.
Resource: https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous is when different tasks run on a single thread, one task running after another finishes in sequence. In contrast, asynchronys code is when tasks run independently of other tasks, where each can be run using different threads without having to wait for other tasks to finish. The advantage of asynchronous code
is that the current flow of operations will not be interrupted by code in queue.
Resource: https://www.youtube.com/watch?v=vMfg0xGjcOI
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
It's hard to reason when each of the asynchronous code will execute.
Asynchronous code will not necessarily run in the order in which you wrote them,
because execution depends on how fast the files load from the server.
Resources:
https://www.quora.com/What-does-it-mean-that-Javascript-is-asynchronous
https://www.youtube.com/watch?v=vMfg0xGjcOI
```
