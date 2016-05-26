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
<!-- your answer here -->
The event loop is responsible to look at the stack and the webapis task queue. Every time the the stack is empty it hands the new task from the top of the queue and put its on the stack (that will make the code actually run).

If something needs to be handled by an web the event loop will send this block of code to the webapi and clear therefore the stack. Now a new thing can be operated at the stack and the webapi is handling it’s request at the same time. Nothing gets blocked. Once the webapi is ready it will send its answer back to the task queue. From there it will get hardened from the vent loop back to the stack once the stack clears.

The stack can only handle one thing at the time, but through the event loop things can happen at the same time, also called async.
```

In your own words, describe the difference between sync and async:

```md
<!-- your answer here -->
- sync : running code from the task queue one after the other
- async : making use of the event loop and handling several requests at a time

```

What are some benefits and disadvantages of async?

```md
<!-- your answer here -->
Sync:
- can block the browser, meaning that the user can’t click anything while the server is processing a request. - Leads to slow webpages, that nobody likes.

Async:
- you end up with a lot of callbacks. Code can start looking not very clean compared to Phyton that uses sync.
- code gets very complex

Source: https://www.quora.com/What-are-the-disadvantages-of-using-Node-js
```
