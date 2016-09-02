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
An event loop stores requests and their callbacks. The way it works is by determining the order of such requests.

source: readings provided
```

In your own words, describe the difference between sync and async:

```md
sync = server can process only one request at a time.
async = the server can proccess multiple requests at a time without compromising the execution of others.

source:  http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
```

What are some benefits and disadvantages of async?

```md
Benefits: async is obviously faster since it works requests do not need to be answered one by one. Disadvantages: we can obtain unpredictable responses or the whole process may or may not take longer.
```
