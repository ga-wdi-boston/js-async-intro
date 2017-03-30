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
The event loop handles placing things on the call stack after it is clear. As code
is executed the event loop looks at the call stack and passes it the next thing
it has in its queue. This allows for code to execute at separate times out of order.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous code executes in a specific order everytime as in traditional compiled
languages such as C ++. The code happens one line at a time in order
Asynchronous code can execute in different orders and not necessarily at the same time.
Such as is the case with an event listener for a click. The code is read into the
browser by not execute in a specific order or at a specific time. The event loop
helps with making sure code is executing when it should and not conflicting with
other processes that may be currently running.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage is it allows for much more dynamic code. The disadvantage is that
you have to consider what is executing and when. I.e. - blocking the call stack.
If you write code and do not consider the call stack you may have a piece of code
that takes a long time to run that is holding up other code you want to execute
such as a click or user interaction of some kind. Careful consideration of the
call stack is needed with highly complex code so that the page can still render in
between code exection and not waiting for some process to finish- as an example. 
```
