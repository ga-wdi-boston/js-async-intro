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
<!-- The event loop is the pattern of read, load and execute that our code goes through to load and exceute on the page. Js is a single thread language and will load each item in our code one by one through the call stack and into the runtime envrironment throughout the event loop. The event loop is essentially everything that's being loaded into the dom, the order of the queue and what is being loaded when. I dont understand it fully yet, but it's clear how important and understanding of it is as what you build becomes more complex and to save you a lot of time in debugging issues.


  -->
```

In your own words, describe the difference between sync and async:

```md
<!--
async kind of takes in all your orders and starts to construct them into the DOM  more simultaneously, which is great if you want to just get everything loaded altogether but can be problem with elements that are dependant on each other. sync will load everything in order, one by one. I'm assuming thats what single thread means, processes everything in a single thread of events.



 -->
```

What are some benefits and disadvantages of async?

```md
<!--A disadvantage is that if you don't stack things effectvively, you can have things running slow, like if your code si bogged down with too many animations. If you have javascript functions that depend on eachother, they won't load in order and you will likely run into some problems with async--unless you use a script loader that makes sure they're executed in order and not just when they're loaded (when the order is ready).

The benefits are that if the first elemeent in the call stack times out or errors, it will still process and load other eleements instead of halting the whole process. With async you can stil be parsing out the html and css elements while the javascript loads, as opposed to waiting for one after the other. If you have a script that comes after the css elementsm it will wait for the css to be available before it loads the script, making the process much longer, whereas if you put an async attribute on that same script, it will already load and execute without waiting for the css elements to load, I think.



 -->
```
