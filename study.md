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
The event loop watches the call stack and allows the task queue to run a task only when the stack is clear.
```

In your own words, describe the difference between sync and async:

```md
Sync fills the stack with functions that have to run in order, while async exports tasks
to the web api in order to clear the stack (temporarily).
```

What are some benefits and disadvantages of async?

```md
Async is beneficial because it can decrease load time by prioritizing tasks/functions.
That being said, it can also confuse the run order and lead to possible task queue flooding.
```
