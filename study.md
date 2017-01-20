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

The event loop system that manages callback functions stored from the web API. When a callback function that has a asynchronous feature is executed it gets moved from the stack to the web API ultimately to the callback queue where it is stored later to be executed. When the all lines of code have been executed and the stack is empty the event loop will select the first element stored in the callback queue and put it on the stack where it is executed. This process will continue until there is nothing left in the callback queue.

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

Sync is a system of code execution that will execute each line of code one at a time and waits for the API call to return before continuing. Until a response is received fro the API the application will not continue until the previous code is executed.
Async is where execution continues in a program and the program does not wait for the API call to return from the server. This is done by placing a callback function towards the end of the code. This allows for more a user friendly and fluid UI as the user is not constantly waiting for lines of code to be executed.

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

The main advantage of async is that the user experience is more fluid as the program or site is not held up waiting for each line of code to executed. A disadvantage of async is that the code can become very complex as the use of callback functions are essential. 
