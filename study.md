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
The event loop allows the stack in javascript, which is syncronous, to execute code asyncronously. Web APIs handle some tasks. When they are completed, the code/info is pushed onto the task queue. The event loop is the function that determines the JS callstack is empty and then passes code from the task queue onto the callstack to then be exectuted/presented to the user.
```

In your own words, describe the difference between sync and async:

```md
Sync means that things are executed in exactly the order they are put on the stack. You can easily predict in what order things will be executed. Async means that things wont necessarily be exectued in an fully predicatble manner. Some other API is managing some tasks, which are then queued after they are completed, and the order of code execution can be unintuitive. 
```

What are some benefits and disadvantages of async?

```md
A benefit is that processes that require retrieving info from the internet are passed to the web APIs, so that you continue to execute other code without halting your stack calls. Another benefit is that things taking a long time on the stack can block the update of the page but not allowing the event loop to pass a render. This can make your webpage appear frozen or inactive. A disadvantage is that you can't be certain exactly when some code will be executed by the callstack, just that it will sometime in the future. >
```
