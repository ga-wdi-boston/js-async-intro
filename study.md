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
The event loop is the order which Javascript is executed and helps keep track of what to run next.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Synchronous JavaScript refers to how each block of code is processed one step at a time.
Asynchronous JS allows us to run code independently and essentially lets code multitask by
allowing event handlers to actively listen for an event while moving on to the next block of code.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Best part about async is that it makes a webpage run faster, instead of waiting for one thing to execute at a time.
It can also do multiple things without breaking.
I can't really think of any downsides of async...
```
