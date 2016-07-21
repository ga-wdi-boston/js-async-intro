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
Functions in JavaScript represent a block of code that is designed to perform certain task. JavaScript can perform only one line of code at the time. Functions can pass their return values to the next function and be presented in a chain like scheme called call stack. Executed functions are placed on top of each other in the order they get called/executed.

The question is what happens if we have the same while loop that is triggered by a callback function to perform some tasks within the browser? Browser gets stuck even though loops are synchronous in JavaScript. It gets stuck for variety of reasons depending on the actions they are required to do, but mostly because those actions take some time to be performed.

The solution for this is making asynchronous callbacks where we run some code, we pass a callback function and we run the code later. A good analogy for this is setTimeout() method that delays actions within that method. Our code still performs one line of the code at the time while another code is waiting to be executed. This is called event loop.
```

In your own words, describe the difference between sync and async:

```md
Synchronous code runs in the order the code gets executed.

Asynchronous code changes the main program flow, and lets other lines of code run after asynchronous call without waiting for asynchronous code to get executed.
```

What are some benefits and disadvantages of async?

```md
Benefits: we "can" run more than one line of code at the time. This isn't completely true since JavaScript allow us to run one line of the code at the time, but by running asynchronous call in the background, we can still execute our code that follows the asynchronous call.

Disadvantages: complexity. 
```
