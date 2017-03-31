# JavaScript Async Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

These studies focus on the differences between Asynchronous Code, and
Synchronous Code. For the most part, you can think of the differences as the
following. However, the readings will go into much more detail on the
differences and patterns of each.

Synchronous Code - operations the occur sequentially: ask db for data; wait; db gives data; do something with data.

Asynchronous - operations that may start in a certain sequence and may end in any permutation of that sequence while unrelated stuff happens in between.

## Required Readings

-   [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
-   [Understanding Asynchronous JavaScript](https://www.youtube.com/watch?v=vMfg0xGjcOI)
-   [The Restaurant](https://www.codeschool.com/blog/2014/10/30/understanding-node-js/)
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until the section on fibers)

## The Event Loop

In your own words, describe the event loop and how it works.
This loop is how JS keeps track of which task to work on next, be it a sync or an async task.
The Event Loop is a queue of callback functions. It is the part of JS that is responsbile for actually invoking the callbacks. When an async function executes, the callback function is pushed into the queue. The JavaScript engine doesn't start processing the event loop until the code after an async function has executed. The Event loop  looks at the call stack, and at the task queue. If the stack is empty it takes the first thing off the queue and pushes it onto the stack to run it. The Event loop waits till the stack is clear before it can push a callback onto the stack.



```md
<!-- your answer here -->
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md

A synchronous task will execute within the browser until its completion unlike an asynchronous task that can be stqarted and then put aside until a later time while the JS engine gets started on the next task the synchronous list.

Asynchronous programming refers to a style of structuring a program whereby a call to some unit of functionality triggers an action that is allowed to continue outside of the ongoing flow of the program. JavaScript is a single-threaded execution environment. If you want anything to happen as a result of asynchrony, you’ve got to do through callbacks  because only there’s one thread of execution.

Asynchronicity = you run some code, give it a callback, and we run that code later..that is why lines 3 and 5 below run later.
Here is a good example of synchronous and asynchronous code that I found on StackOverflow that explains the difference nicely:

  console.clear();
  console.log("a");
  setTimeout(function(){console.log("b");},1000);
  console.log("c");
  setTimeout(function(){console.log("d");},0);

  A request comes in, and JS engine starts executing the code above step by step or synchronically. The first two calls are sync calls. But when it comes to setTimeout method, it becomes an async execution. But JS immediately returns from it and continue executing, which is called Non-Blocking or Async. And it continues working on other etc.

  The results of this execution is the following:

  a c d b



## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```
The big benefit is: More responsive applications for users.

You need to be careful while writing async code because if you accidentally write a synchronous piece of code it'll block the main thread (as it's single threaded) which in turn affects the performance of your app.
Another disadvantage is Error handling becomes more complicated.
Thirdly writing async code is more complex.

source: https://thenewstack.io/async-officially-coming-javascript-year/


```
