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
Javascript can only run one thing at a time. When we are runing a code, the functions
are stacked up in order waiting to be run by JS. If some of the functions have events that are
not able to processing immediately, then they will be moved to Web API and wait until be activated. Once JS finishes the work in stack, it will call them back
from callback queque, after the functions have been activated in WEB API.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync means there are two different systems doing the same thing simultaneous. Async means two systems work independently at the same time.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async can solve the disadvantage of the event loop, which JS can not take a new
codes till the callback queque codes has been finished processing. But its disadvantage
is the new input codes will be process indepently from the previous one, it may mess up the
order of the whole process or haveing missing data error occur. 
```
