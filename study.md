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
The event loop helps asynchronistic code to be executed.  It orders the completed asynchonicstic code so that it will execute once all the other, synchronistic code is run```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
blocking or synchronicstic code takes all the time and attention of the server and no other events can be interacted with while that code is running.  Asyncronics code can be waiting for an event or response to finish processing while other code runs and events are engaged with at the same time. Web Apis help run code asynchronistically, and get arond the fact that javascript is single thread.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantages of async are that is allows you continue to use a webpage while waiting for a response from a server or doing some other function that takes a long time.  Without it interactive web pages would move really slowly.  A disadvantage is that it is less clean, and can lead to users being confused about what is happening to their requests and possible resubmitting something many times while they are waiting for it to run.```
