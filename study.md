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
The event loop is where callbacks are invoked. The event loop will invoke callbacks from the task queue and pass them into the stack when the stack is empty.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Async code means the code can be executed at anytime in any order. It often means that there is a signal/event that will trigger the code to execute. Multiple async code can be exectuted in parallel.
Sync code means the code is executed in sequence. A subsequent line of code will not execute until the preceding code is finished executing.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async advantages involve the parallel execution of code where tasks can be passed to other task handlers at the same time. It can simplify and streamline complex operations into small pieces.

Disadvantages of async involve unexpected/unintentional layers of complexity if callbacks are not organized/documented proprerly.
It can lead to unpredictable response times and performance.
```
