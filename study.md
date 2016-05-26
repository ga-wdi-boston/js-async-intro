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
The event loop is sort of like a parallel processing stack that recieves code
from the main stack to be executed later. When the required conditions are met,
the code is executed and then removed from the event loop.
```

In your own words, describe the difference between sync and async:

```md
Sync processes requests in order before proceeding to the next executable code,
possibly leading to hangups. Async has the event loop that can 'store' running
code or functions listening for events in order to allow later code to be
processed.
```

What are some benefits and disadvantages of async?

```md
Async better for transmissions that occur at irregular intervals, and is more
simple to set up than sycn, but has a large 'overhead', where a lot of the
information only stands for controlling purposes.
```
