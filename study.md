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
Javascript can only run one operation at a time.  Slower, longer calls can
be queued and thereby allow a faster load time.  The event loop watches for the
stack of Javascript to be clear and then loads queued functions back into the
stack.
```

## Synchronicity and Asynchronicity

In your own words, describe the difference between sync and async.

```md
Sync has things run in the order they were queued at, whereas async bumps the
order around.
```

## Async Advantages and Disadvantages

What are some advantages and disadvantages of async?

```md
Async allows for a faster load time by allowing more complex callbacks to be put
off until later.  It also keeps potentially long responses (especially from AJAX
calls) from holding up other functions that do not need to wait.  All our
studies for this have been praising asynchrony, so finding a more balanced view
was a little tricky.  My google-fu was able to suggest that the biggest problem
with asynchrony is that you're basically sending users an incomplete page.  Normally
this is not a huge deal, but if there's a particular function that's critical to
your app and youv'e delayed it... sure, your user can see the page, but they can't
actually use the page, which causes all but the most saintly of users to hulk out.
```
