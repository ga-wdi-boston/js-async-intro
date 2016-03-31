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
Because JS can run only one line of code at a time, it processes requests in the order it receives them. When an event has a settimer or a funtion that requires reading from another or something else considered 'blocking', it essentially holds up the line the for the next call to get processed. When a call is made, if a callback function is used, JS can execute the function, but execute the callback function at a later time, which means it can continue on processing the next the lines of the code. The event loops comes into play when all of the lines of code in the call log are complete, the function that was called previously in the callback can excecute.


```

In your own words, describe the difference between sync and async:

```md
Sync means calls are processed in the order received.
Async means it can initiate/trigger a call but execute at a later time. So the output of a call third in a seven lines of code may not executed until after seven completes.
```

What are some benefits and disadvantages of async?

```md
The benefit is that your browser is not held up by tasks that are time consuming and can to move on to the next ones.
A disadvantage would be that additional codes/checks are needed if you need data to process and complete in a particular order.
```
