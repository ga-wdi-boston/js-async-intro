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
The event loop is responsible for invoking callbacks. The point of this is when
async calls are completed, they return an event. The callbacks listen for the
event and allow the function to continue.```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous means that the browser cannot handle any events whatsoever until
the first event has triggered. Also can be termed blocking. Asynchronous
on the other hand can be initiated then move on to other tasks while waiting
for the event to complete.```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Pros: Allows your application to continue functioning while waiting for an event.
This allows your code to run more fluidly and can queue up a function while
waiting for the stack to clear.
Cons: I didnt find many but I would say if there is a delay timer, it isnt a
gauranteed time to execute but a minimum. So if a delayed function is in a queue
it could hold up things while its waiting for the delay.
```
