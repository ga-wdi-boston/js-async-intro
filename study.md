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
JavaScript is run line by line, as a result of this browser will be runing the code acording the stack structer. However, when systems tyries runing a web Api it gets out of the stack and gets into que. However, while this process is happening browser does not stop runing the code and runs the following code. When our stack is clear then the code in the que will be run by the browser.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync is doing one thing at one time and async is doing mutlip;le thing at the same time.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantage of astnc is when we have code which needs time to be executed won't be blocking our site because it will be getiing in to que. 
```
