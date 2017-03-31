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
The event loop is a place where a callback gets placed once a response is
recieved from a async request.  The callback then will be pushed to the stack
once it is empty, where it will then be executed.
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronicity is the process of putting(pushed) work on a call stack in the order in
the calls happen. Once a call is done it is removed(popped), removing the next
call on the stack once it executes. This process continues until till there is
no calls remaing.  This is a single threaded system, potentially slowing down
making a page seems slow, while it is processing all the calls.  In contrast
asynchronicity calls are put on a stack and are executed on individual threads
letting the other calls continue to be processed at the same time.
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The main advantage is allowing several things to happen at the same time and not
blocking execution of other calls. A disadvantage is if several calls are
executed at the same time you cannot guartenend when the various calls will return,
if your code is dependent on one call finishing before another you will most
likely have a bug.  We accomplish async via JS, if it is turned off in a browser
we can not use this feature.

http://www.jscripters.com/ajax-disadvantages-and-advantages/
```
