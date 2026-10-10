# Reflection

## Question 1: What did you learn about multithreading from this assignment?

I learned that multithreading allows a program to use multiple threads to perform different tasks. In this assignment, I learned how Java threads can simulate process execution. I understood that Round-Robin scheduling gives each process a limited time to execute. I also learned how the ready queue manages the order of processes. The Thread.start() method begins thread execution, while Thread.join() makes the main thread wait for the current thread to finish. This assignment helped me understand how threads and CPU scheduling work together.

## Question 2: What was the most challenging part of this assignment and why?

The most challenging part for me was implementing the waiting time feature. At first, I did not understand how to calculate the time a process spends in the ready queue. I also found it difficult to know exactly where to add the new methods and variables. The program contains several methods, so I had to be careful when making changes. I needed to understand what happens when a process returns to the ready queue. This part took more effort because waiting time must be measured during each execution round.

## Question 3: How did you overcome the challenges you faced?

I overcame the challenges by working on one feature at a time. First, I reviewed the original code and tried to understand the important methods. Then, I added the required changes step by step. When I was unsure where to place code, I checked the surrounding methods before continuing. I used the console output to verify that each feature worked correctly. Finally, I tested the complete program and confirmed that the priority values, context switch count, and waiting time summary appeared.

## Question 4: How can multithreading concepts be applied in real-world applications?

Multithreading is useful in many applications that perform several tasks. For example, a web server can use multiple threads to handle requests from different users. A media player can use threads to play audio while responding to user commands. Threads can improve responsiveness because some tasks can continue while others are waiting. Scheduling helps organize how threads receive CPU time. This assignment helped me understand why managing threads is important in real operating systems.