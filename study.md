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
<!-- An event loop is a loop function that once called upon runs through a loop until conditions are met. The loop is only executed when the event that is attached to the loop is acted upon. Even loops invoke callback functions.-->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!--
Sync flows with the normal coded flow of JS, while async flows out of order. Async is run only after all normal flow has taken place, and it can contain actions or functions that can run parallel to one another.

"Asynchronus is when you cant count on one thing to finish executing before another thing."-->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!--
Advantages:
  Async does not have to follow regular flow of JS
  Multiple actions can take place simultaniously with async JS
Disadvantage:
  You cant return asynchronis JS
  You cant assign it to a variable
  You also can not error handle async JS
Possible Advantage AND Disadvantage:
  Current code will never be interrupted by async JS code-->
```
