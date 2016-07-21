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
the event loop is a step in the process of an application running on your
computer. when you pass callback functions as arguments into other functions,
your application can move on to another task and let the device's memory finish
the first function. this allows your application to run faster and smoother.
once the output is ready from the first function the event loop will trigger
the callback function so the application didn't have to wait for it to be ready.
```

In your own words, describe the difference between sync and async:

```md
sync would be writing your code so that your application will have to wait for
output before it can finish the task and move on to the next one.

async code allows it to initiate a function and let the cpu finish it so your
app doesn't have to wait for the output before moving on.
```

What are some benefits and disadvantages of async?

```md
async will help your applications to run faster and not 'freeze' while waiting
for output.

if your application doesn't rely on I/O. this was the only real bit i could find
in regards to it not being suitable but not entirely sure what that would even
mean in terms of an application.

used the provided link and video and also found a couple stack overflow queries
```
