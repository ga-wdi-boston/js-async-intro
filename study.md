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
<!-- The event loop is a processing manager. If there is something the task queue
it will check the stack, and if the stack is empty is will pull something from the queue
and push it to the stack.
source: https://www.youtube.com/watch?v=8aGhZQkoFbQ -->
```

In your own words, describe the difference between sync and async:

```md
<!-- Sync means that the code executes all at once. While async means that functions
get pushed to the api and once complete, get pushed to the queue and if the stack is
empty then code from the queue gets pushed to the stack.
source: https://www.youtube.com/watch?v=8aGhZQkoFbQ -->
```

What are some benefits and disadvantages of async?

```md
<!-- the benefits of async are that it allows the browser to render the screen inbetween
code instead of freezing the screen until the stack is empty.
The disadvantages of async are that it overall takes longer to execute code that if it were
sync b/c you need to wait for the stack to be empty before the async code can execute.
source: https://www.youtube.com/watch?v=8aGhZQkoFbQ -->
```
