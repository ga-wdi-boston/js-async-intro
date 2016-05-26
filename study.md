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
The event loop is initiated when conditions are met that signify that an event it has been
told to listen for has been initiated. The event loop handles the event according to its
set specifications and then once the event is completely executed, will execute the next event.
However, other processes are not interrupted nor stopped while the event is being handled.

Sources: http://www.tutorialspoint.com/nodejs/nodejs_event_loop.htm, https://strongloop.com/strongblog/node-js-event-loop/
```

In your own words, describe the difference between sync and async:

```md
Sync is short for synchronous and basically means all events are executed in order and handled one
at a time. Async, or asyncrhonous, means that a request can be handled and processed without interrupting the current activity going on in the browser.
```
source: https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Synchronous_and_Asynchronous_Requests

What are some benefits and disadvantages of async?

```md
For the most part, async is preferable as it allows for more flexibility and a dynamic user experience.
However, sync is good for scenarios when a few processes need to be handled before the amalgamate of the
data returned should be passed to the broswer. Basically, async is better for interactive websites and
for handling complexity, sync is better for tasks that benefit from a more rigid structure in their execution.
```
