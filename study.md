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
The event loop in Javascript checks for when the call stack is clear and then pushes the first callback
in the task cue to the stack.
souce: https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

In your own words, describe the difference between sync and async:

```md
Sync processes happen one after the other in the order you wrote in your code.
Async processes run callback functions in the background while the rest of the
code completes, rendering once the other code has completed and the call stack is clear.
source: https://www.youtube.com/watch?v=8aGhZQkoFbQ
```

What are some benefits and disadvantages of async?

```md
Async makes for a more seamless UI since the user is not waiting for each process
to finish before the next one starts. It allows access to resources that are slower
to respond without disrupting the rest of the script. The disadvantage of async
is that it's less intuitive in what order your code will run; it is also not
supported by a few older browsers such as IE 8/9.
sources: https://www.youtube.com/watch?v=8aGhZQkoFbQ, https://www.codeschool.com/blog/2014/10/30/understanding-node-js/,
https://www.igvita.com/2014/05/20/script-injected-async-scripts-considered-harmful/
```
