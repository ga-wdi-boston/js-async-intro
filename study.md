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
The event loop organizes callback functions and lets them know when they should be run. Essentially the call stack is what dictates whether or not a callback function can be run and the stack has to be empty for a callback function to run. The event loop will look at the stack, see its empty, and say the stack can run
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync is like basic JS which means one thing can only happen at once and it has to happen in order. The order in which these functions is run is also on the call stack.

Async utlizes web APIs and pushes functions to them. The way I understand it is that this is useful for long functions.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The benefeits of async is that it allows longer functions to be "set off to the side" while the rest of the stack can perform the necessary tasks.


This may be subjective for disadvantages but callback functions seem to make everything more difficult(at least in my brain) which would make async harder to troubleshoot.
```
