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
<!--
The event loop determines if it is appropriate to move a task from the task queue to the stack for processing. The event loop determines this by first looking at the stack and then looking at the task queue. If the stack is clear, the event loop then takes the first task on the task queue and moves the task from the task queue to the stack (which then runs that task). Tasks are added to the task queue after being completed by the web API.

Additional Resources: https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop

 -->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!--
Synchronous Task: A task that will occupy the handler continually until that specific task is completed. Regardless of how long it takes that task to be completed, the event handler will wait to move forwards until that task is completed. Synchronous functions are conceptually linear, they require that all information is available in order to move forwards (i.e. they cannot start a task and wait for it to be completed).

Asynchronous Task: A task that can be initiated and moved past while it is being processed. After the task has been processed, the task's completion event will be triggered and will let our JavaScript know that the task being processed is ready to be used.

-->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!--
Benefits:
  1. Reduces the waiting time associated with slow resources.
  2. Optimizes computing time by initalizing processes, leaveing them to complete, and retreiving them when ready instead of waiting the whole time and not moving forwards in the mean time.
  3. Increased capabilities when nesting functions (we have can save the processing time associated with certain tasks until absolutely necessary).

Disadvantages:
  1. The dangers of callback hell: enough callbacks and code is almost impossible to follow.
 -->
```
