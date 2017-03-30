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
The event loop determines which parts of your code will run at one point.  Each piece of code is run by being placed on the stack in proper order.  Once each piece of code is run, it is moved off the stack and the next piece of code runs.  However, asynchronous code, particularly code with set timeouts, is a bit different.  Asynchronous code is rendered by web APIs, which waits until the alotted time with that code.  In the meantime, the synchronous code on the stack will still be running.  When the timing or execution of the asynchronous code is complete, that task is put in the task queue, and any other asynchronous events follow it.  Nothing in the task queue is run until the stack is empty.  After that, the event loop moves each event from the task queue to the stack, where it is run.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous code is code that is run entirely in the stack with no timeout or other events that would cause that code to be delayed.  Synchronous code always runs in the order of the program.  Also, synchronous code occuppies all of Javascript's single thread, meaning that if Javascript is stuck on one line of code, the browser can't do anything else.  Asynchronous code consists of certain events such as AJAX and timeouts that don't run with the normal flow of the code, instead being run on web APIs if timed, and then put in the queue.  Asynchronous code is a part of sepration of concerns where certain events are taken out of the main flow of the code.  On some systems, asynchronous code runs similar to paralell computing where multiple threads of code run simultaneously.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The primary advantage of asynchronous code is that asynchronous tasks can be initiated and put aside while other code runs.  This is somewhat of an exception to the fact that Javascript is single-threaded.  However, asynchronous code that performs functions in the background will not fully execute until the Javascipt stack is empty.  This means that asynchronous code will not necessarily flow with the program as a whole.  This makes it harder to figure out when and how your code will execute, which is a disadvantage of asynchronous code. 
```
