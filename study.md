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
The event loop is the process by which applications can send requests to servers
and not hold up the entire client-side, it designates a callback to be executed
once the output from the request is ready, but in the mean time the program
continues and does not get blocked.
```

In your own words, describe the difference between sync and async:

```md
Synchronous refers to actions being done in order, while asynchronous means they
 can be done outside of a strict order. In other words, if our code sends a
 request to retrieve data, the program can continute with other operations while
  we are waiting for the response, and trigger a callback to be executed
  asynchronously (out of order) when that reponse is completed.
```

What are some benefits and disadvantages of async?

```md
Benefits: it allows us to continue with other operations while we are waiting
for requests to be processed and responded to by the server.
Disadvantages: programs that have heavy computation but not a lot of
input/output requests would not perform so well in an asynchronous manner
since the performance of the callback function once the response is received
would hold things up (even though they can continue doing things while waiting
for responses, once the response is received and callback starts to execute,
the program cannot do more than one thing.) 
```
