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
The event loop is the mechanism through which JavaScript manages tasks to be completed. Because the language is single-threaded, only one block of code can be executed at a time. When a block of code with a callback is read, it is "placed to the side" in an event queue. This ensures that the browser doesn't get hung up on a block of code, preventing the rest of the program to progress. When the program finishes and the "stack" is cleared, the item at the top of the even queue is the next thing to be processed.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Syncronous code is exectuted in the order it is written. One block of code will not execute until the block of code before it completes. Asynchronicity allows for multiple blocks of code to run in parallel, or to set code aside for processing later. Code written using a non-blocking model allows for code blocks with callback functions to be executed at a later point or run in parallel if the task is taking a long time to complete. This allows the browser to move on to the next code block without getting hung up.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages - A user can continue to interact with a page if a particular request is taking time to process. If a button click makes a call to the server and it's taking a long time to pull back the request, the user can continue to interact with the application.

Disadvantages - You cannot guarantee events will happen in the order in which you wrote them, or the exact timing of an event. When events with a set delay are queued, the set delay is more like a "minimum expected delay". If there are other events queued up ahead of the event with the delay, it will take longer for the event to complete.
```
