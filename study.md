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

The event loop handles a queue of asynchronous callback functions. The event
loop waits until the call stack is empty, then pushes one function from this
queue to the call stack so it can run.

```

In your own words, describe the difference between sync and async:

```md

Sync means each instruction is executed in order. The next line of code can't
run until the previous line has finished running. If the previous line takes a
long time to run, the next line has to wait.

Async lets us run a line of code and set an action to take when it completes,
then move on. We can say "do something, and when that finishes, do something
else" and then move immediately on to "do a third thing." When the first thing
finishes, the "something else" will run, even if we've moved beyond that into
other lines of code/other actions.

```

What are some benefits and disadvantages of async?

```md

Pros: Async lets us move more quickly and avoid having to wait until something
is done before doing the next thing. If one thing gets hung up, our whole
program doesn't necessarily get put on hold. For example: if we click a button
to make an AJAX request and it's taking a long time, our browser can still
"un-depress" that button and let us move on, rather than freezing/hanging
until the request completes.

Cons: It looks like error handling is more complicated in asynchronous
programming? Also, you can't necessarily predict or control when callbacks
execute. A callback passed to setTimeout will run a *minimum* of the specified
number of milliseconds later, but not exactly—it could be more.

```
