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
The event loop moves the task at the front of the queue to the stack when
it sees that the stack is empty and the queue is not. It is how a asynchronous
callback function ends up back on the stack once it returns from the web API.
```

In your own words, describe the difference between sync and async:

```md
sync runs on the stack, one at a time, so it blocks the stack e.g. if it is slow, nothing else
can happen. This is especially bad because it will block the event loop, which
is what moves the screen renders from the queue to the stack, which means that
the page won't actually look like it updates at all while the long thing is
running.

Asynch means that something is running in some web API and that can be happening
in parallel to the stack, so it doesn't block the stack or event loop. This is
important for potentially slow things, like network requests. It will end up back
in the stack once it gets to the front of the callback queue and the event loop
puts it on the stack (when the stack is empty).
```

What are some benefits and disadvantages of async?

```md
The key benefit, as described above are that slow-running code can be used
without blocking the stack.

A disadvantage is that if you queue something that takes a long time, at least
in a single-threaded language like JS, you will block the event loop and nothing
else can happen. I think this would still happen in a synchronous function
though, so I am not sure if it is really worse.
```
