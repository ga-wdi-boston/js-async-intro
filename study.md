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
The event loop helps javascript and the web browser process tasks.  Javascript can only perform one action at a time.  Sometimes it has to perform an action that involved making a request to a server.  While it is waiting on the server for a response, it can't perform other tasks.  So, the browser includes some tools that can process these requests, allowing javascript to continue without having to wait for a response.  When the request to the server is processed, the browser cant just return the response to javascript because javascript is probably in the middle of something, and it would mess it up.  So, the browser sends the response to a queue.  The event loop checks to see if javascript is in the middle of a task, and if it isn't the event loop sends the first thing in the queue to javascript.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
sync is when the code is processed all on the same thread.  Only one event can be processed at a time, so an event must finish before the next one starts.  Some code runs very fast on most computers so this is fune for them.  async is when actions that take time (a complicated process or a request to a server) are placed into a different thread to that the original thread can continue processing, then the actions are integrated back into the first thread.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage is that requests to servers can be processed separately from the javascript processing the code.  This allows the code to continue without having to wait for the request to process.  Also, if the single thread was waiting on a request and the user tried to click some things, the actions would be queued up and execute as soon as the request was processed, causing mayhem.  A disadvantage to async is that on a simpler program, async can take longer to complete tasks than sync because if it is simple, the sync can process code very quickly.
```
