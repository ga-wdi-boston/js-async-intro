# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.

```md
<!--The event loop allows you to side bar and que timed/slower resolving events in order to keep the stack clear for quick resolving parts of your code to resolve. As slower resolving parts of your code that enter the stack are called upon they're put in a task que, and when they stack is clear they're called to resolve. -->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!--Sync is when things execute in a concurrent timeline.  Async is when things sort of don't happen in concurrency. It splits your executables into multiple threads. The quick resolving items in the stack will resolve as they come, but things that would block or take longer are qued in a task que. When the stack in cleared javascript will look at the que and resolve what is in the que until something else comes into the stack. Basically it will only resolve the other things in the que when there are no longer things to do in the present stack. This means you can not count on when those things will resolve. -->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!-- Async is great for not blocking up the que with things that take longer to resolve and for allowing javascript to run multiple things at once to speed up the process. The major negative part, is when writing code to include async returns you can not count on when they will resolve. This is because javascript will only attempt to resolve them when there is nothing else left in the main stack.  -->
```
