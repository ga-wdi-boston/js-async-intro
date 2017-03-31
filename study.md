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
-event loop- looks first to the  call stack for "work", if the call stack is empty then the event loop will look at the task queue for work. If there is something on the task queue, the event loop will push that thing onto the stack so it can be ran.

-You can set something to time 0, so that you are immediately adding something to the task queue and waiting to run that piece of code until the call stack is cleared.

```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous code is code that executes one block after the other. Can't do anything before the previous code completes

Asynchronous code is code that can be accessed or ran later i.e. out of order.
```

## Async Advantages and Disadvantages



What are some advantages and disadvantages of async?

```md
Advantage- website will operate more seemlessly to end user.



Disadvante- more complicated for coding. Potentailly to run into concurrency issues. Front end could be trying to call an object before the backend is done updating it, so the front end would display the wrong info to user. Performance of the backend matters.
```
