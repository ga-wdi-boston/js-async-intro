# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.

```md
<!--An event loop invokes callbacks. Non-blocking inputs and outputs release an event when their calls are complete, and these events trigger the return... So event loops put returns on the back burner until the event is triggered.-->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
<!--Synchronicity means JavaScript runs each section of code at a time, like in a single line... JS works with each section of code until it's done. Asynchronicity allows JavaScript to mimic multi-tasking by putting returns on hold until JavaScript needs it (event loops do this for JavaScript and signal an event when the returns need to be put back into the queue)-->
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
<!-- advantages: You can run code more efficiently you're letting it "multitask"
disadvantages: callback hell and event loop blocks... you back up the return queue or you stack up so much you don't even get to the queue (since JavaScript won't really look at the queue unless there's nothing else to do)... you can get out of this by mimicking synchronicity (having an asynchronous function "wait" to meet up with the synchronous function)-->
```
