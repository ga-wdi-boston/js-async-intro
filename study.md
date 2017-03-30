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
The webapi pushes the callback on to the task queue.  The event loop then looks at the stack and the task queue.  If the stack is empty, it takes the first thing on the queue and pushes it onto the stack, which runs it.

Sources:

Required readings

https://nodesource.com/blog/why-asynchronous/

http://www.cs.unc.edu/~dewan/242/s07/notes/ipc/node9.html

http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean

http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/

http://altitudelabs.com/blog/what-is-the-javascript-event-loop/


```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync is when things occur one at a time.  One request or process blocks another request or process until it is completed.

Async means that processes operate independently of each other.  It is non-blocking.  One request or process is not dependent on another request or process to be completed.  This most commonly takes the form of Ajax.

Required readings

https://nodesource.com/blog/why-asynchronous/

http://www.cs.unc.edu/~dewan/242/s07/notes/ipc/node9.html

http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean

http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/

http://altitudelabs.com/blog/what-is-the-javascript-event-loop/

```

## Async Advantages and Disadvantages

Advantages:
-Tasks can occur independently of each other.  The browser does not lock up while one task is being processed.  Instead, one task can be initatiated, and then other tasks can occur before that task is completed.

Disadvantages:
-Identification and tracking of errors is more difficult.
-It can be hard to identify specifically when a task will be initiated and completed.

Required readings

https://nodesource.com/blog/why-asynchronous/

http://www.cs.unc.edu/~dewan/242/s07/notes/ipc/node9.html

http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean

http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/

http://altitudelabs.com/blog/what-is-the-javascript-event-loop/


```md
<!-- your answer here -->
```
