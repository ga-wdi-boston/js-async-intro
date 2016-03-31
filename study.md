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
When code is being run asynchronously and a callback is sent to the task queue, the
event loop chooses the right time to release the callback into the stack.  This happens
only when the stack is empty meaning the rest of the code has been run.
```

In your own words, describe the difference between sync and async:

```md
When something is executed synchronously, the processor is working on task 1 until
it is finished.  Then it turns its attention to task 2 until that is done and so on and so
forth.  If the code is being executed asynchronously,  the processor will work on some of task 1, then
perhaps some of task 2.  It might return to task 1 for a while and then begin on task 3.
The processor, which can only work on one thing at a time, does not need to finish
the task before moving on to another.
```

What are some benefits and disadvantages of async?

```md
Async provides a much better user experience.  The browser won't become unresponsive
while it waits for code to be executed.  Writing async code can lead to nested callbacks
and thus, hard to read code.
```
