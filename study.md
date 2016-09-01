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
<!-- your answer here -->
```

What are some benefits and disadvantages of async?

```md
<!-- your answer here -->
```
