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

```md an event loop takes a funciton from the call stack and moves to the event
stack where it waits/listens for the event to occur. When it does, it adds the
result to the event queue, which waits until the stack is clear to add the
function result to it.
source (http://altitudelabs.com/blog/what-is-the-javascript-event-loop/)```

In your own words, describe the difference between sync and async:

```md asyc allows for requests that have not completed to be 'stored' and queued
not directly on the stack, making it possible to move onto the next task. sync
requires every task to be completed in order of being called.
source (https://www.youtube.com/watch?v=8aGhZQkoFbQ) ```

What are some benefits and disadvantages of async?

```md async will let you continue to run code while you're waiting, but that has
the side effect of letting things run 'out of order', maybe in a way you weren't
expecting.
source (https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)```
