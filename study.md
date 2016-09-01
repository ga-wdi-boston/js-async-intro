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
So JavaScript can only execute one function at a time, and each function
goes into the 'stack'. Once a function is complete, it is removed from the top
of the stack.

However, the browser and various APIs have their own 'stacks' of sorts, which,
while they can't directly affect the main JS stack, do hold the callback functions
and wait for the event emitter. Once it receives that event emitter, the
callback is passed to another queue, kind of like a waiting line.

The event loop then checks to see if the JS Stack is empty. If it is, it will
take the first callback waiting in the queue and pass it to the stack, effectively
running that callback function. If the stack is not empty, it will wait until it is clear
before it begins passing any callback functions to the main stack. This allows code
in the stack to continue operating while we are 'waiting' for an event emitter to trigger a callback.
```

In your own words, describe the difference between sync and async:

```md
Synchronous means that a piece of code is executed in the order it is written, with
only one function happening at a time. The previous function must complete before the next
function can start.

Asynchronous allows us to queue up other code to run at some point in the future, usually
when some event is triggered. This lets other code continue running synchronously in the meantime, so things don't slow down.
```

What are some benefits and disadvantages of async?

```md
The biggest benefit is that async makes things way faster, and helps prevent one
aspect of a program or site from slowing everything down while we wait for it to finish.

There don't seem to be many disadvantages from what I understand, except that async does
also operate on a 'queue' of sorts, meaning that if we have a number of callback functions
waiting in the queue, they can get backed up and then fire off at once, causing some of
the slowness we were trying to avoid in the first place.
```
