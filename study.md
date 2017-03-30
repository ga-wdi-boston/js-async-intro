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
the event loop looks at the stack.  if the stack is empty, the it will grab the
first item off the task queue and push it to the stack.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
with sync, when an action is started, only that action is working until it finishes.
with async, multiple actions can be worked on and completed
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
advantage, more work can get done.  less bottlenecks
disadvatage, harder to code for.  the flow of you program may execute out of
order.  cannot count on 1 thing happening before another
```
