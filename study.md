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
The event loop is a process that handles functions processed through web apis to prevent web page slowdown on the front end.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync places everthing in one big stack to be executed one after the others. Async allows the offloading of certain tasks to other services to prevent the stack from being blocked.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
While async does allow for a faster, smoother front end experience, values returned from async functions will not always be accesible right away making them harder to work with. Aditionally, the event que can get congested just as the stack can so it is important to think about how much data is offloaded.
```
