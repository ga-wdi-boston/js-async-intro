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
Event Loop: looks at the stack and look at the task queue, if the stack is empty
it takes the first thing in the queue and put it in the stack so it runs.

```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
async: is where you can't count on one thing to finish your program.  async task
can be initaited and put aside for later while it starts on the next task.

sync: wont respond to any event till it completes its first handler.  Task
that takes the full attention are called synchronous
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages:
Requests need not be targeted to specific server.
Service need not be available when request is made.
No blocking, so resources could be freed.
Could use connectionless protocol

Disadvantages:
Response times are unpredictable.
Error handling usually more complex.
Usually requires connection-oriented protocol.
Harder to design apps
```
