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
The event loop is part of the precess that is in place the help the UI remain fluid.
Since JS is a single thread code, code will pile up on the stack and run in order.
If a particular function take a long time to run it will slow the browser while
it runs. Callback functions are asynchronus, so they will move off the stack into
web API to run. Once they ar run they go to the task queue. The event loops looks
at stack and task queue. Once stack it clear it will take the first item in the queue
and put it in the stack to complete it's function. The event loop is part of the process
that allows for a better more fluid UI.
```

In your own words, describe the difference between sync and async:

```md
Sync functions will run one after another no matter how long each one takes. This
can slow the browser down. Asynchronus functions will "run" in webAPI to help rest
of the code run faster.
```

What are some benefits and disadvantages of async?

```md
Async advantages: UI is better. Reatime data heavy apps will run smoother and faster.
Aysnc disadvantages: It hard to write the code correclty and hard to debug. 
```
