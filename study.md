# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop takes function calls from the callback queue and pushes them onto the stack. The event loop is what invokes callbacks.
```

In your own words, describe the difference between sync and async:

```md
Synchronous processing does things one at a time, in order, and processes on the stack (not in the webAPI).
Asynchronous processing can transfer certain (async) tasks to the Web API to
wait for something to happen while the stack goes and continues executing other
functions.  When a function in the WebAPI executes, it is pulled onto the
callback queue and will eventually be pushed to the stack by the event loop.  
```

What are some benefits and disadvantages of async?

```md
Advantages: You can divide workload between the webAPI and the stack.  Certain
functions are inherently slow (and sometimes infinitely slow) because they wait
for either user input or input from another part of the system before executing.
Async allows us to continue running other functions that are not waiting for
furthur input or an event to trigger, allowing for less hangup time and a
smoother user experience.

Some disadvantages of async are that you can find yourself in deeply nested
callback hell, and it can be hard to debug where something went wrong when you
have callbacks going through many different files at many different layers of
abstraction.  There might be issues of getting your code to execute in the order
that you want it to run in, but in that case, you probably should be using
synchronous programming.  
```
