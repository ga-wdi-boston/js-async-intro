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
The Event loop sits and watches the stack to see that all of the job are done.  When they are it will then check the task queue to see if anything is there (or has completed after the other jobs have run).  If there is something there it moves it to the stack to run.  If not then nothing changes.  In a sense it 'mimics' a synchronous thread.

RESOURCE:  Video
```

In your own words, describe the difference between sync and async:

```md
Async means that the processes or code being run is done so one at a time.  Sync means they are done in parallel or concurrently (at the same time or side by side.)

RESOURCE:  Prior knowledge and the event loop video

```

What are some benefits and disadvantages of async?

```md
An immediate advantage is that one thing completes at a time before the next bit of code runs.  This could benefit resource (i.e. memory allocation, etc).  A drawback is that if one call or bit of code gets hung up then the entire thing is hung up and the user (or program) experiences a delay.

RESOURCE: Prior knowledge and video.
```
