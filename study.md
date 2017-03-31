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
When the call stack is empty ,the Event loop passes task from the task queue into the call stack.  These task were originally passed from webAPIs into the the taskqueue and they are executed sequentially.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Syncronous code is javascript that is written and executed in order.  The code remains in the call stack and is executed in order only once the previous action has been completed.

Asyncronous code is the use of web APIs or feature browsers to delay execution of a task.  This allows you to delay execution of a function until after the other tasks in your call stack is clear.  This can help you avoid locking up your website.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
An advantage of async is that it allows the browser a chance to redraw and not lock up the website.  It allows you to execute functions when things are ready allowing you to simulate using Javascript as a multithread language.

The disadvantage is that it can be somewhat complex and messy to implement.  Poorly designed function also can clog up the task queue.
```
