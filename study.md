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

The event loop is a way for a application to request something then move on to another task while its request is processed.  It works with a event listner so when the event (like the request comes back complete) the script invokes a call back function to complete the next part of the task it started.

In your own words, describe the difference between sync and async:

Sync is done in order one after another.  You cant do anything else until you complete all the steps in sync.
Async is the opposite.  It allows you to cut in and out of line.  You can do one thing and then start another thing.  When the first request completes it goes to a waiting area like a side bar then is pushed back to the stack when its clear.

What are some benefits and disadvantages of async?

Benefits are that it can alow your application to be more responsive, faster, plus it uses JavaScript.  THe disadvantages could be that you dont know how to use it properly. You can load the waiting area with to much.  You might want to have certin processes returned before others.  I cant find to many disadvantages besides that it is still a relativly new technology. 
