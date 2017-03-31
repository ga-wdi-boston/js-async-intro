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
The event loop is the process where it will wait until there is nothing in the
stack and then pulls the first thing from the task queue and puts it on the stack
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
sync is the process of doing tasks one at a time in order and waiting until that task
is done until you start the next task

async is the process of doing tasks in order but not waiting until the tasks
are done before starting the next task. Then returning the result of the task when it
comes back.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
advantages of async is that it can run all the code and not have to wait for tasks
that are taking a while to complete. The disadvantages of async is is the complexity of it
if you dont watch out you might end up in callback hell!
```
