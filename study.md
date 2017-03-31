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
When we run our code, it executes by running one piece of code at a time through the stack. However, if there is any sort of delay put onto a piece of code, this causes it to be pushed to the web API and then eventually to the queue. Once the stack is done executing the code within the stack, the event handler will then pull whatever piece of code is left waiting in the queue and execute it at this point.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
With synchronous code, the code executes line by line in order, with only one thing happening at a time. With asynchronous code, code may execute out of order or concurrently in separate threads.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
An advantage to asynchronous code is that you can manipulate the order in which your code executes with the queue and event loop. It also allows multiple things to execute independently which can speed up the running of your code. I imagine a disadvantage would be that it can sometimes be difficult to keep track of the order in which code is executing and make sure things happen when they should be.
```
