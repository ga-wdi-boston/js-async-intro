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
The event loop is what pushes evnts/tasks from the Queue to the Stack. It keeps tasks lined up in the order it recieves them, and then pushes them one by one to the stack, when the stack is empty.

Source: the video linked above.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
executing tasks in sync is to execute them one at a time, waiting for the previous one to end - every time.
Executing tasks asychronously starts and runs tasks along side other tasks.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
async:
Some benefits are that a slow task, or a task with a timer can be run without holding up other tasks.  By putting the webapi to work as well, that can help speed things up. It may allow for easier use of multiple CPUs?

some disbenefits are that it may effect the order in which error codes are registered which may lead to confusion. It may make the system harder to maintain or less reliable.


```
