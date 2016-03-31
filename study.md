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
The event loop is part of the browser (or node.js) that periodically checks for tasks
in the task queue that have been placed there by Web APIs (part of the browser or node.js).
In addition to checking for queued tasks, the event loop checks the state of the stack.
If the stack is empty at the time of the check, the event loops places the first queued
task onto the empty stack. [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
```

In your own words, describe the difference between sync and async:

```md
Syncronous (I don't know the right word to use next) systems/execution/processing? is the processing of
tasks based on their execution order in the source code and their position on the stack. If you have
a processing intensive task, it blocks the stack, leading to other key tasks, e.g., the rendering of
the web client in client land, pausing until the long task completes.

Asyncronous processing allows for longer tasks to be deferred until shorter tasks have
been completed and the stack is empty.
```

What are some benefits and disadvantages of async?

```md
Disadvantages:
1. Execution order may not be as intuitive since tasks are added to the stack after completion
and after the stack is empty, rather than in the order they are written in the source code.
2. Please let me know if this is correct, but it seems like a task might get "lost" or never
"complete" or never be handed off to the task queue from the Web APIs, leading to more
difficulty in handling exceptions and timings.

Advantages:
1. Relatively slow tasks (I/O, image processing, intensive computations) are allowed to load
once the stack is free from smaller tasks, leading to a more responsive system (at least until
the task has been added to the stack by the event loop.)
2. Not sure of a second advantage besides increased responsiveness and performance. I would appreciate input here.
```
