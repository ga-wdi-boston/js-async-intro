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
The event loop has one small role in the grand scheme of asynchronous programming.
While functions that exist in the native engine of Javascript are executed,
those that are not native such as Webapis (e.g. Ajax requests, DOM apis) are moved
to a task queue. Until the stack is cleared – in other words, when all the functions
are done running – the event loop does not kick in.

The event loop looks at the stack and the task queue. If the stack is empty, it
takes the first thing in the queue and pushes it into the stack, effectively
running that piece of code.

```

In your own words, describe the difference between sync and async:

```md
The difference lies in order of execution. In sync programming, functions are
executed from top to bottom, a strict order is maintained. One operation follows
the next, slowing down the whole process. On the other side of this is async,
which basically enables parallel execution, or concurrent execution. While
something is working, the program is not stopped, instead you're allowed to
perform another action.   
```

What are some benefits and disadvantages of async?

```md
Async is allows performance without halting the execution of a program. An example
is the browser rendering. Through async programming, the browser has a chance to
render the page in between elements. It does not block the event loop by stacking
code that is slow to process. In terms of sync, the browser faces a time constraint
when it comes across Javascript. The browser cannot render the page if code exists in the call stack.

Async might not be necessary for every type of application built such as those requiring
heavy computation and very little input and output (fetching resources outside of the app).
```
