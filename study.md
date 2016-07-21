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
The event loop is a way of evoking the callback function. It does this by using
the same ready function we use when making sure HTML is ready for JQuery. 
```

In your own words, describe the difference between sync and async:

```md
Async and sync are two  different ways of handling functions and event loops.
Async steps through each step as it completed and cannot move onto the next step
until the previously one is done. Sync allows all these steps to be done at the
same time, which allows them to all be sent through at the same time.
```

What are some benefits and disadvantages of async?

```md
Sync is good for things which are time sensative, material which you want to be
completed at the same time and sent at once. Async is good for material that
depend on each other and their result, therefore they rely on the previos action
before they know what to do with the information at hand. They need that
information to complete the task.
```
