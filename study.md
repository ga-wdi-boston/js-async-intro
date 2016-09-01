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
The event loop is the middle man between the task queue and the call stack. The
event loop is constantly watching the call stack and when the stack is empty,
it sends the first thing in the task queue to the stack to be called.
```

In your own words, describe the difference between sync and async:

```md
Sync means running each line of code one at a time and waiting for each call to
fully process before moving on to the next one. While async isn't really
allowing multiple things to happen at once, it kind of is. Async allows the
call stack to remain unblocked, which leads to much better performance for
reasons outlined below.
```

What are some benefits and disadvantages of async?

```md
Async keeps the call stack unblocked, which is very important, especially with
functions that take a long time to process. Processes that take a long time,
like callbacks that are called in loops or upon receipt of network responses,
can be called in ways that don't interrupt the ability to render the page. The
page can only be rendered when the call stack is empty. If the call stack is
waiting for a long loop to finish or a network request to process, the user can
experience a frozen webpage, which may lead them to click wildly and add even
more functions to the stack. Instead, these long loops and network requests with
callbacks can be sent to the task queue. Once in the task queue, the event loop 
will wait until the stack is empty and the network request has been processed
to send these callbacks to the stack. This gives the page time to render and run
the rest of the file while the longer processes are put off until they can be
run in a more manageable manner.
```
