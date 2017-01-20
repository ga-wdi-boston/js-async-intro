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
An event loop is important in explaining the order in which functions are run in the browser (which impacts the speed of calling these functions).  It can be thought of as ordering tasks in a to-do list.  Because a browser cannot run multiple functions at the same time (i.e. single threaded), these functions are put in a callback queue.  Then, the event loops moves these functions in a specific order to the call stack, which runs the code.  With code that has a function run for an event that can occur multiple times (e.g. 'scroll'), the function is run multiple times.  The callback queue can be flooded.  It is at this point that the operation (i.e. synchronicity and asynchronicity) comes into play (see below).

Source 1: https://www.youtube.com/watch?v=8aGhZQkoFbQ
Source 2: https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/

```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
For sync, rendering is blocked as the code is being executed.  This is because the render queue has to wait until the call stack is cleared.  Therefore, rendering is blocked which slows does the execution of code.

For async, rendering can take place in between functions running in the call stack.  In other words, the render queue is not waiting for the call queue to clear before rendering.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage of async is that functions can be rendered as the code is being run (rather than waiting until the call queue is cleared).  This speeds up the process of rendering code.

One disadvantage of async is if you want all the code to run before rendering occurs.  For instance, if you want a page to entirely load before javascript is rendered.  Here, async, which renders along the way, is a disadvantage.
```
