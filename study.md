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
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until section on fibers)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop is what invokes the callbacks in asynchronous processing.  When an
asynchronous call is completed, it's sent to a task queue.  The event loop waits for
the call stack to be clear and then take the responses from the front of the task queue,
and invokes the callbacks from their corresponding intial functions (which pushes it to
the call stack).

Resources:
What the heck is the event loop anyway? - Philip Roberts
https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

In your own words, describe the difference between sync and async:

```md
Sync - Only one request can process at a time.  That request must be fully processed
before another can begin.
Async - A request can be triggered and then other requests can be handled until a response
comes back for the initial request.

Resources:
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
```

What are some benefits and disadvantages of async?

```md
Async is beneficial because it helps user experience by not locking up the browser
or causing code to be really slow.  A disadavantage is that the callbacks required
can cause complicated code and lead you into "callback hell."

Resources:
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
```
