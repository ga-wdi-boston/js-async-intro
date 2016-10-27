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
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until section on fibers)

## Event Loop?

In your own words, describe the event loop and how it works?

```md
The event loop is something that monitors the stack and the queue. When there is something that it waiting to be run in the queue and the stack is empty, the event handler moves that something into the stack.

resources used:
https://www.youtube.com/watch?v=8aGhZQkoFbQ
https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop
```

In your own words, describe the difference between sync and async:

```md
In general, javascript can only process one piece of code at a time. With sync javascript has to wait for the result of each process before it can move on to processing the next piece of code.

With async, javascript gets help from apis and the queue, so that it can process the next piece of code while the first piece of code is being processed, somewhere else, and then javascript will be notified when the result from the first piece of code is ready.

resources used:
https://www.youtube.com/watch?v=8aGhZQkoFbQ
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

What are some benefits and disadvantages of async?

```md
Async allows your code to be processed more quickly, but you can still have issue with your browser being stuck trying to render new pages if there are too many returns on the queque without adequate delays to let the page re-render.

resources used:
https://www.youtube.com/watch?v=8aGhZQkoFbQ
https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```
