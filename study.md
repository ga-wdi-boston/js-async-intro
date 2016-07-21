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
https://nodesource.com/blog/understanding-the-nodejs-event-loop/

From my understanding, the event loop is what is dealing with all of the javascript.
When an asynchronous code is sent to the API and gets what's requested, it is then sent
to the queue waiting for the stack to clear.  Once the stack clears the event loop then brings this javascript into the stack.

I'm probably wrong about this.

```

In your own words, describe the difference between sync and async:

```md
http://rowanmanning.com/posts/javascript-for-beginners-async/

Synchronous code will read in a sequence, line by line; each line isn't executed until the one before it finishes. This can cause slow and sometimes painfully long rendering time. Asynchronous code will bring statements outside of the main program flow, which allows other code to be read while it is recieving the requested pages; making it have
a faster rendering time.
```

What are some benefits and disadvantages of async?

```md
The obvious benefit is that it can make for a better user experience by lessening
the amount of rendering (or speeding up the page).  Too much asynchronous code can
actually lead to less performance and more complex code.
```
