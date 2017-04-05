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
<!-- the event loops takes all the functions that are exectuted and puts them
in a queue, and executes them after the callbacks are completed.  -->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!-- sync requires JavaScript to run only one task at a time, but to wait until
the task is complete, before moving on to another task.

async allows tasks to be executed, but then JavaScript can move on to another
task while that one is completed -->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!-- an advantage of async is that the browser will not be locked up while waiting
for a function to complete.  this will allow other operations to happen concurrently.

the biggest disadvantage was referred to as "callback hell" in one of the articles
we read.  to me, it sounds like you can get bogged down with increasingly more
complicated callback functions that will eventually drive you insane, unless
you've written exceptional pseudocode and can decipher it later on. -->
```
