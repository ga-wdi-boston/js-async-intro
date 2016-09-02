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
JavaScript runtime performs other tasks while waiting for asynchronous
operations and their callbacks to execute. Messages to be processed, along with
their callback functions, are stored in a message queue. JavaScript runtime
goes through the queue, finds the message(a click event, a function in said event,
etc.), and executes the callback.
http://blog.carbonfive.com/2013/10/27/the-javascript-event-loop-explained/
```

In your own words, describe the difference between sync and async:

```md
Sync: Client will get a callback only after the server receives AND processes
the request to oad the JavaScript. It takes longer for the webpage to load because it stops DOM
construction while the request is processed.
Async: Client will get a callback after the server has received the request.
The browser continues working normally while the request is processed. The
DOM will continue to be constructed and thus the page will load more quickly.

https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Synchronous_and_Asynchronous_Requests
https://www.nccgroup.trust/uk/about-us/newsroom-and-events/blogs/2015/july/what-are-the-benefits-and-drawbacks-of-loading-javascript-asynchronously/
```

What are some benefits and disadvantages of async?




```md
Benefits: Browser doesn't slow down while a request is being processed. DOM
construction continues. It is more efficient.
Drawbacks: There is no guarantee as to what order JavaScript files will be
executed on the page. Sometimes different files are dependent on one another,
and in this case sync is the better option.
```
