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
https://developer.yahoo.com/blogs/ydn/part-1-understanding-event-loops-writing-great-code-11401.html

The event loop is a natural behavior of how javascript executes.  The event loop is a continuos event listener but also conducts and keeps events organized as they run.

Having worked with hardware, normally there are two parts to the main script:

void setup() {} and void loop(){};

setup occurs when the hardware is first powered on or resetted. and whatever is put into the loop just runs continuously over and over again. In order to add more structure to the hardware performance, common practice is to put getStatus() and getMessage() in the loop. The combination of the inherent loop(){} along with getMessage(){} is the quivalent of a js event loop. Except the messages are coming ffrom the same client.

If an even happens, it's forwarded to getMessage(event) which witll then execute the event associated with the event that was passed. From there, asyn vs sync behavior determins how the program will execute.

```

In your own words, describe the difference between sync and async:

```md

http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
example:
loop(){
event1();
event2();
event3();
event4();
}

event2(){
eventa();
eventb();
eventc();
}

Synchronous: the loop would begin at event 1, move onto event 2 which has to fire events a,b,c and complete event 2 before moving onto event 3.

Asynchronous: the loop begins at event1, moves onto event2 but hands event 2 off to the operating system to complete while the computer moves on to event 3 and 4. later the result of event 2 returns when it is complete.
```

What are some benefits and disadvantages of async?

```md
Sync was the bane of my existence when working with low-level programming for microcontrollers and arduinos.  Everything runs step by step and the program cannot move to the next step until the previous event has executed all of its callbacks.  Benefits for async is that more than one function can execute- this is super important when stauses need to be logged.  If an event is fired, that even will cycle through callbacks and during that time, a getstatus report is on hold as well as browser repainting. In the case of hardware, lots of times somethting goes wrong during the process and you have no clue because status reporting is halted during the execution of a different function. Async takes care of all of that by allowing more than one event or function to occur at the same time.

Downside to async is that it is more difficult to codunct and maintain exect control and timing.  Sync is perfect for a master slave, print message receive message relationship.  You always know exectly what events are occuring at a given point in time.


```
