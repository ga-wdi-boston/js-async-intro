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

In your own words, describe the event loop and how it works.

```md
The event loop has one simple job: it "looks at" the stack and
the task queue, and when the stack is empty, it "pushes" a callback from the
task queue onto the stack. This is so that other code can execute while a
setTimeout function, for example, is taking a few seconds to run, without holding
up the stack. If I understand the video correctly, this is why Javascript is
referred to as a "single-threaded" language, which I believe means code can only
be executed along a linear timeline. So basically the event queue allows a piece of code (a callback in most cases, I think), to "hang out" without disrupting--or holding up--
the sequence of code that it's in.

```

In your own words, describe the difference between sync and async:

```md
The difference between sync and async is that synchronous code has to be executed
in order, waiting for the previous task to finish before moving on to the next task.
Asynchronous code, on the other hand, can be executed "out of order," meaning that
you don't have to wait for a big slow block of code to execute before moving on to
the next block of code. Tasks can run simultaneously, and are moved to the stack only
once they are ready to be executed, speeding up the entire process of rendering
things in the browser.

I've come up with an analogy for async, which has helped me understand it--if it
is a bad analogy, please let me know! It goes like this: let's say there are four
women runninga  relay race, where a baton has to be passed from one runner to the
next. They are each in place at a predetermined place on a track, waiting for the
previous runner to pass the baton to them so they can run their leg of the
race. But while they are waiting for the baton, each woman is not frozen in space
and time: she can move freely, do some jumping jacks to keep warm, stretch,
whatever. But she is still waiting for the baton in order to "execute" her portion
of the race. So in async multiple tasks can be occurring simultaneously, but
each bit of code--or "leg of the relay"--won't be added to the stack until it is
ready to go, thus not holding up the flow of the UI.
```

What are some benefits and disadvantages of async?

```md
An advantage of using async would be if you need to render a lot of code in a
broswer where certain blocks of code take awhile to execute, like animations,
for example. With async, these slow chunks of code don't block the stack, because
the event handler allows them to run on the web API while other code is being
executed, and then pushes them back onto the stack once they are done. On the
other hand, a disadvantage of asynchronous programming is that the semantics
of how things tie together are complicated, creating an easy place for errors
and/or bugs.
```
