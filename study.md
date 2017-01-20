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

```md
The 'event loop' is responsible for invoking callbacks. In node.js, as a primary example, code execution is reliant on event loops acting as listeners for events(or changes in the state), as can be seen in the DOM, and loop to callback functions that are executed when a specific event happens. Basically, I am thinking of events as user interaction with a web app/page and the event loop is the response(in the form of callback methods) to this user interaction.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
When using a query to retrieve data, sync is when the command is not executed until each operation in the query has been executed. Async is when operations are all executed at once, without waiting for the query to finish retrieving information from the database.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
There are both advantages and disadvantages to async. Advantage wise, async allows for more immediete response, so reueste information is recieved much quicker. Continuing to work through code  whilst retrieving data might be more efficient, but it also, at least from what my novice developing skills have determined, seems to create harder to read code. Though this will likely change with time, async's use of callbacks and their given valid arguments seems like a lot to keep track of when I am trying to understand the proper pattern that facilitates this system in the first place. Node.js 'apparently' helps make async code flow in a more readable fashion.
```
