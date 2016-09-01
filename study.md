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
The event loop is a part of the browser machinery that decides when functions
from the callback queue are allowed to run. It's like a smart little revolving
door that only lets a callback function onto the stack (where it will be
allowed to actually execute and do its thing) if the stack is empty.

In conjunction with other tools that push functions into the callback
queue (instead of putting them directly onto the stack), the event loop allows
the browser to delay the execution of (possibly) slow functions until faster
functions have already finished executing.
```

In your own words, describe the difference between sync and async:

```md
Sync is where every function call goes onto the stack immediately and stays
there until it is resolved.

Async is where a function can send a callback function into some sort of
separate mechanism (like a third-party web API), which feeds it into the
callback queue. From here, the event loop feeds the callback into the stack.

Async allows a developer to differentiate between slower functions that should
be delayed, and faster (or simply higher-priority) functions that should be run
immediately.
```

What are some benefits and disadvantages of async?

```md
Benefits
-Slow or low-priority functions can be kept from running until fast or high-
priority functions have been executed.
-We can (sort of) run multiple threads of code simultaneously. There is still
only one stack, but the event loop lets us keep a queue of function calls
separate from the browser's runtime stack.

Disadvantages
-Added complexity seems like a possible disadvantage. In order to delay a
function's execution, we have to embed it as a callback function. Writing a lot
of callback functions potentially makes our code difficult to read and debug.
```
