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
The event loop is how javascript allows you to do multiple things at once.
This is instead of having to call a function, wait for completion, and then
continue to the next action. For example, a webapi (like timer) is called and
completes shortly after. Once complete, rather than jump (perhaps into the middle)
of the stack - the callback moves to the task queue. The event loop is a simple
but important piece of this. The event loop will keep checking to see if the stack
is empty - and if it is - the event loop will push the first item from the task
queue into the stack.

Source: https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

In your own words, describe the difference between sync and async:

```md
Sync are tasks that are performed and must be completed before continuing.
Async tasks are those that can started and then move onto the next one -
checking in later on the result (callback).

Source: https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```

What are some benefits and disadvantages of async?

```md
The main benefit is that you can significantly speed up the overall
run time of your app by running tasks asyc. The downside is you
are introducing a significant degree of complexity (e.g. callback hell).
That being said, there are some mitigation strategies you can use
to help make the complexity manageable (e.g. promises).

Source: https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
```
