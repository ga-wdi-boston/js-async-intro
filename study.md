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
The event loop is something that looks at the task queue and the stack and puts the queue onto the stack.```

In your own words, describe the difference between sync and async:

```md
Sync code is performed at the same time, meaning it processes tasks one at a time from the stack. async means that more than one process can occur, or 2 processes are relagated to different parsers.```

What are some benefits and disadvantages of async?

```md
A benefit from async is that it bypasses a step, in a way, as it can operate on stacks while something at the bottom of the stack takes a long time to process. Async gets processes to the api and queue quicker than sync. A disadvantage to asynch is that is is not streamlined across languages and browsers to there is a disconnect in the req response cycle. ```
