# Development Log
**Operating Systems – Assignment 1**

## Entry 1: GitHub Repository Setup

**Date:** October 9, 2026  
**Task:** Setting up the GitHub repository.

**Work Done:** I forked the starter repository and renamed it to OS-Assignment1-Yazan-Alduaiji. I also added my student ID to the Java code and opened the project in Visual Studio Code.

**Challenge:** I had some difficulty understanding how to use GitHub and connect the repository with VS Code.

**Solution:** I followed the assignment instructions step by step and checked that the repository was ready for development.

**Time Spent:** Approximately 45 minutes.


## Entry 2: Understanding the Starter Code

**Date:** October 9, 2026  
**Task:** Reviewing the original Java code.

**Work Done:** I reviewed the Process and SchedulerSimulation classes. I learned how Round-Robin scheduling works and how processes use the ready queue and time quantum.

**Challenge:** Some Java methods and operating system concepts were new to me.

**Solution:** I reviewed the code carefully and ran the original program to understand its output.

**Time Spent:** Approximately 1 hour.


## Entry 3: Adding Process Priority

**Date:** October 9, 2026  
**Task:** Implementing Feature 1.

**Work Done:** I added a priority variable to the Process class and assigned random priority values between 1 and 5. I also displayed each process priority when it entered the ready queue.

**Challenge:** I had difficulty finding the correct locations for adding the new code.

**Solution:** I checked the methods step by step, added the required code, and tested the program to make sure the priorities appeared correctly.

**Time Spent:** Approximately 1 hour and 15 minutes.


## Entry 4: Counting Context Switches

**Date:** October 9, 2026  
**Task:** Implementing Feature 2.

**Work Done:** I added a static counter to count process execution turns. I increased the counter each time a thread started running and displayed the total at the end of the simulation.

**Challenge:** I needed to understand where to place the counter inside the scheduling loop.

**Solution:** I placed the counter after Thread.start() and tested the program. The output showed a total of 12 context switches.

**Time Spent:** Approximately 35 minutes.

---

## Entry 5: Tracking Waiting Time

**Date:** October 9, 2026  
**Task:** Implementing Feature 3.

**Work Done:** I added variables and methods to track the waiting time of each process using System.currentTimeMillis(). I also created a summary table showing the process name, burst time, and waiting time.

**Challenge:** I had difficulty understanding how to calculate waiting time when processes returned to the ready queue.

**Solution:** I used startWaiting() when a process entered the queue and stopWaiting() before execution. I tested the program and checked that the waiting time summary appeared correctly.

**Time Spent:** Approximately 1 hour and 20 minutes.