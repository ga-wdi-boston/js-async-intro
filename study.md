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
The event loop is a way for a program to run code when it can't predict when that code will need to be run.  When JS reaches a line of code that can't be run at the moment it is reached, it puts that line into a separate queue which will be completed at a later time.  Things that go on this queue are the results of event handlers and functions that are passed as callbacks to setTimeout() and I'm sure other things.  Once JS reaches a point where the main stack is empty the event loop will resolve the code in the queue by putting it on the stack to be run.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous execution of code means that each line runs in the designated order and takes as much time as it needs to complete.  While synchronous code is executing, any inputs will not register and delays will complete in their entirety before the next line of code can be run.

Asynchronous execution of code means that more than just the single-stack execution of code can happen while running a program.  Asynchronicity allows users to perform actions on their UI while code is executing and to not lose those actions because a different line of code is executing at that moment.  It also allows setTimeout() to not completely interrupt the flow of the program, but to allow the program to keep running until the function passed to setTimeout is ready to be run.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage of synchronous code is that it is completely predictable.  All results have been calculated.  The disadvantage is that synchronous code cannot create compelling, interactive programs.

Asychronicity is a difficult concept to understand, but it allows programmers to create much more interactive and functional programs.  A disadvantage is that any delays caused by the program are a MINIMUM delay.  There is no way to tell how much longer after the minimum the program will take to resolve the lines of code on the queue because some items on the stack that need to get resolved first might be complicated, heavy pieces of code.
```
