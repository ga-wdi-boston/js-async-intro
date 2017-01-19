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
Node processes are single threaded and non-blocking.  Because they are single
threaded, they can only process one operation at a time.  However, because it is
non-blocking, it can make IO calls outside of the application and remember its
context so that, when it can return to handle the IO call response.  The event
loop makes this possible.
Essentially, the event loop works like a stack.  When an IO operation
returns, a message is placed at the back of a message queue containing the
callback passed to the IO operation calling function.  The callback functions
are then passed onto the execution stack.  They execution stack, in turn,
looks to the message queue for new messages when the stack is empty.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
In synchronous programming, operations are executed in sequence until completion.
Asynchronous program introduces "events" to organize execution of blocks of code
out of sequence.  In practical terms, this means that the developer must be aware
of the fact that execution order and flow is dependent on the timing of operations
outside of his or direct control (such as the completion of the file read or the
response time of an API.)
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async programming allows for the creation of dynamic applications capable of
reacting to user activity.  On the server side, it powers fast web servers capable
of handling large amounts of traffic with relatively limited resources.

One major drawback of the async paradigm is the complexity it introduces.
"Callback Hell," as its popularly known, arises when the programming task relies
on a series of sequential asynchronous operations each of which depend on the
outcome of the former.  It can be difficult to handle errors and maintain a
mental model of what the code is doing in the waterfall of callbacks.
```
