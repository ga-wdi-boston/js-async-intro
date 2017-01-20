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
Basically, the event loop waits for an event to trigger and place its callback to a
task queue. Then, the callback will be processed when the "stack of functions"
finish processing. Please advise if I am wrong. I tried using MDN and other youtube videos
to get a better understanding of this, but am still unsure as how it actually works.

```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
sync - at the same time
async - not at the same time
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
The advantages to async is that its fast, won't get held up, can still do "stuff"
while processing. As for the disadvantage to it is that a function could be executed
before the prerequisites to the function executes, thus, will potentially return an
unexpected result.
```
