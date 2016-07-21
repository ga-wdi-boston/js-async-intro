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
The event loop in JavaScript is responsible for sending a previously requested and completed task back from the task queue to the call stack to be performed, once the stack is empty of other requests.  This task was first called, then sent to a webApi to be continue being processed while other JavaScript code is being read. Even though JavaScript is single threaded, apparently multiple processes can occur at once, they just need to be called one at a time.
https://www.youtube.com/watch?v=8aGhZQkoFbQ
http://stackoverflow.com/questions/16336367/what-is-the-difference-between-synchronous-and-asynchronous-programming-in-node
```

In your own words, describe the difference between sync and async:

```md
Sync in JavaScript is in reference to synchronous functions, which are performed one at a time when code is running.  The browser is unresponsive during this time because JavaScript is single threaded.  This is also referred to as blocking.
Asynchronous functions are non-blocking and they can be started but stored somewhere else while other code is running.
Most of JavaScript I/Os (inputs and outputs) are considered non-blocking, so the idea of async is that those processed can still be taking place while a function is in the middle of being processed.  That function will be recalled via a callback function at some point in the future.
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

What are some benefits and disadvantages of async?

```md
The obvious advantages of async is that complete halting of the browser while waiting for a function to be processed can be avoided or minimized.  Other non-intensive I/O tasks, like HTTP requests, database queries and disk reads can still be done if async protocol is followed.
The main disadvantage of async is that it becomes more difficult to figure out the order in which the JS code will execute.  Some function may not be performed when the developer intended it to, which could result in a program error.  This will depend on the server's query response, which can actually change moment to moment depending on network or latency issues.
Also, when the code is setup to perform async, some code may load before CSS is completed loaded.
https://www.quora.com/What-does-it-mean-that-Javascript-is-asynchronous
```
