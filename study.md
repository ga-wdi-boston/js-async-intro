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
The event loop seems to be pretty key for async programming. Because most callback functions need to operate in sequential order, they need to be stored in order for the Js to to execute the asynchronous code
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync code basically executes one line at a time, going down the list. Async does not do this, and in async code, the code does not necessarily execute in exact sequential order.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
async code does not necessarily adhere to the logic flow we have been covering, meaning that it can execute in unforseen and unintuitive ways. The primary advantage to async is that code executes far quicker, as there are multiple threads handling different elements of the code all at the same time.
```
