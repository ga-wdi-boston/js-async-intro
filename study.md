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
The event loop is essentially a queue that stores requests and their respective
callbacks. The loop then dictates the order of which the requests are to be executed.


```

In your own words, describe the difference between sync and async:

```md
With synchronous execution, the server can only process and complete one request
at a time before moving on to another request. Asynchronous execution is when
the server can process multiple requests as once.

sources: http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
```

What are some benefits and disadvantages of async?

```md
There are many benefits to asynchronous transmission. Most notably, it generally allows for faster service requests because resources are unblocked, and requests need not be targeted to a specific server. However, there are a few disadvantages to async, such as the need for a relatively large overhead, as well as the fact that the request protocol can sometimes result in unpredictable response times.
```
