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
An event loop works as a task manager for Javascript. While one function is running, it keeps tabs on the repsonse and thread it back into the code when it's ready. While the event loop is taking care of that function Javascript is running through the rest of the code.
```

In your own words, describe the difference between sync and async:

```md
Synchronous is when a single piece of code is running and that code requires all of Javascripts attention. The code won't continue to run through the rest of the function until that event is completed. This is also known as blocking.

Asynchronous will allow Javascript to run that piece of code but then put it aside until a later time (for the event loop to deal with) and continue working through the rest of the code.
```

What are some benefits and disadvantages of async?

```md
A common problem with async is callback hell. Some benefits include more fluid UI so that the browser doesn't get stuck performing one event. It's also helpful when
heavy processing needs to take place and may take longer to perform than more simple functions.

Resources used: https://www.codeschool.com/blog/2014/10/30/understanding-node-js/
https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/
https://www.youtube.com/watch?v=8aGhZQkoFbQ
```
