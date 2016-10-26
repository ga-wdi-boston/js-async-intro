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
-   [Javes!](https://www.discovermeteor.com/blog/understanding-sync-async-javascript-node/) (until section on fibers)

## Event Loop?

In your own words, describe the event loop and how it works?

```
The event loop is...ok, so you're at an amusement park, you're in line for the rollercoaster.  Rollercoaster runs, does its thing, people get off, gates open and next people get on, rollercoaster runs, does its thing, people get off, gates open and new people get on, etc etc.  The event loop is the gates, allowing people to do what they are there to do, ride the rollercoaster.  Too many people get on at once, bad things happen, the event loop holds people (tasks) back.
<!-- your answer here -->
```

In your own words, describe the difference between sync and async:

```md
Sync handles one operation at a time, without multi-tasking.  Async handles one operation at a time, WHILE multi-tasking.
<!-- your answer here -->
```

What are some benefits and disadvantages of async?

```md
Advantages are obvious, it doesn't tie up your resources waiting for code to finish.  The only disadvantage that I could find was that it is ore difficult (impossible?) to determine/guarantee the order in which code will execute in certain circumstance.

cite:https://www.quora.com/What-does-it-mean-that-Javascript-is-asynchronous
<!-- your answer here -->
```
