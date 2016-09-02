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
<!-- your answer here -->
Everytime an event is fired it is added to a queue and waits for the action to
be completed. Once it is done processing, it will return back to the event and wait
for it to be initiated again.
```

In your own words, describe the difference between sync and async:

```md
<!-- your answer here -->
For a sync loop we need to wait for a task or callback to finish before we can
do another one. Asyn is the opposite where we can do other stuff while the task
or event loop is running.
```

What are some benefits and disadvantages of async?

```md
<!-- your answer here -->
We are able to do more things at once with async callbacks because we do not need to
wait for the task to finish before doing something else. This means the processing
time will be faster. However, it is more complex than sync and requires more memory
to run.
```
