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
Eventloop is the process the holds a task que from a function and wait to place that task into the call
stack after the stack is clear. For example, two people walk into a restaurant and place two orders at the same time -- one person orders a salad, a sandwhich, and a soup and the other person orders a steak. Most likely,
the salad, soup and sandwhich will come first because the length of time to prep/cook those meals is faster than a steak. Meanwhile, other people are ordering meals, and it is being added onto the queue for the kitchen as well. Once the steak is ready, and the server has finished serving a table -- they will finally take it out of the 'queue' and bring it to the customer.

source from reading and video
```

In your own words, describe the difference between sync and async:

```md
Sync is having your code execute, wait, and the move on. Async is having your code excecute, move the slower processing code into a 'queue' to finish computing, execute the next code, and when the code in 'queue' is ready -- execute this after the all the other pieces of code has finished.

source from reading and video
```

What are some benefits and disadvantages of async?

```md
The benefits are that your program will run much faster. However, all of those nested callback function can make
your code complex and if you accidently run a sync function in your code -- it could cause errors.

- sources from readings and this link https://hashnode.com/post/what-are-the-actual-disadvantages-of-using-nodejs-ciibz8fd3017yj3xtxqz1r9hs
```
