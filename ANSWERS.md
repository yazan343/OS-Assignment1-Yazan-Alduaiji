# Technical Answers
**Operating Systems – Assignment 1**

## Question 1: Thread vs Process

A process is a program in execution with its own memory space, while a thread is a smaller execution unit inside a process. Threads in the same process share memory, but separate processes normally have their own address spaces. Threads also have lower creation overhead and can communicate more easily through shared memory. In this assignment, we used Java threads to simulate processes because they are easier to create and manage inside one Java program. The code uses `Thread thread = new Thread(process)` to create a thread for each simulated process.

## Question 2: Ready Queue Behavior

In Round-Robin scheduling, each process gets a limited amount of CPU time called a time quantum. If a process does not finish during its time quantum, it returns to the end of the ready queue. For example, in my output, P6 had a burst time of 2534ms and executed for 2000ms, leaving 534ms. The scheduler added P6 back to the ready queue so it could finish later. This behavior is important because it gives other processes a chance to use the CPU and improves fairness.

**Example from my output:**

```text
P6 executing quantum [2000ms]
P6 completed quantum 2000ms
Remaining time: 534ms
P6 yields CPU for context switch
P6 added to ready queue
```

## Question 3: Thread Lifecycle

A thread begins in the New state when it is created using `new Thread(process)`. It becomes Runnable when `Thread.start()` is called, and it runs when the CPU schedules it. In my simulation, P1 begins its execution and uses `Thread.sleep()` to simulate CPU execution time. While P1 is sleeping, the thread is temporarily in a Timed Waiting state, and the main thread waits using `Thread.join()`. After P1 completes its execution, its thread enters the Terminated state. These stages show how Java manages thread execution during the simulation.

## Question 4: Real-World Applications

One real-world example is a web server that handles requests from multiple users. The server can use multiple threads, and fair scheduling can help prevent one request from using all the CPU time. Round-Robin scheduling can improve responsiveness by giving runnable tasks repeated opportunities to execute.

Another example is a game engine that manages several tasks, such as updating game objects and processing user input. A time-sliced scheduling approach can help tasks receive regular execution time. This is useful because interactive systems need responsiveness and predictable progress. The same idea appears in my assignment, where processes share CPU time through a ready queue.