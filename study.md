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
The event loop is the sequence of how JavaScript handles normal javascript functions, callback functions, and events.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync functions are functions that are executed one at in the sequential order of invocation in the call stack. Async functions are functions that are started and processed (?) outside the call stack, the result of which is then set aside to be returned to the call stack after the normal functions in the callstack are done.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage of async is that it does not have to wait for all other functions in the call stack to process in order to do its own processing. The processing of the async does not block the user from interacting with the browers.

The disadvantage of the async is that it has to wait until the callstack is done with all of its work before it is pulled into the callstack. Also, the returned values cannot be handled without workarounds (promises).
```
