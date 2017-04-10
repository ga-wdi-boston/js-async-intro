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
The event loop is something built into the JS engine in Chrome (V8) that takes tasks and puts them onto a stack executes them and then takes them off the stack in synchronous order. It can only do one thing at a time. The way it can deal with code that takes a while to process (blocking) is by putting those tasks in the event queue. The event queue is like a waiting room in parallel to the main callstack. When pieces of slow/blocking code are finished, they can be put back onto the main stack at the next availabale opportunity, or at a specific time that you as the programmer assign.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync represent code/programming that can execute literally one thing at once, in order, without exceptions. If code is slow, the rest of the code behind it has to wait.

Async is code/programming that utilizes parallel threads so that certain processes can operate separately from others. This way, those pieces of code don't have to wait for others, or don't hold up others themselves if they are slow.

Chrome still has a single callstack, but it utilizes these queues/waiting rooms in order to simulate parallel programs.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Advantages:
-Code is non-blocking/faster
-Service need not be available when a request is made.
-Could use a connectionless protocol if necessary

Disadvantages:
-Response times can be unpredictable, increasing complexity
-Debugging complexity is increased
-Harder to read/more complex to code
```
