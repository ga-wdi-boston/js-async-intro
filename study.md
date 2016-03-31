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
In Javascript, the event loop monitors the task queue and stack elements of the
script message queue.  When the stack has completed all its tasks, the event
loop moves the next task waiting in the task queue to the stack where it can be
completed.

(Sources:
https://www.youtube.com/watch?v=8aGhZQkoFbQ
https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)
```

In your own words, describe the difference between sync and async:

```md
A sync operation can only be run in the stack after the previous one has been completed and cleared.  Async operations can run simultaneously and don't need to wait for other tasks to be completed to be initiated.


(Source:
http://stackoverflow.com/questions/16336367/what-is-the-difference-between-synchronous-and-asynchronous-programming-in-node)
```

What are some benefits and disadvantages of async?

```md
Some benefits of using async are that the processing time for scripts is decreased via allowing tasks to run concurrently, and the css can be run earlier.  Disadvantages include that the order in which scripts are executed can't be controlled which creates issues if files are dependant on each other to run as intended and potentially limits a developer's vision for how code should execute.

(Source:
https://www.nccgroup.trust/uk/about-us/newsroom-and-events/blogs/2015/july/what-are-the-benefits-and-drawbacks-of-loading-javascript-asynchronously/)  
```
