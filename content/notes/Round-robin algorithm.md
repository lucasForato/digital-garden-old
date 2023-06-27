---
title: "Round-robin algorithm"
---
# Definition
The Round-Robin algorithm is a scheduling algorithm used in computer systems and networks to manage the allocation of resources or the execution of processes. It is commonly used in operating systems, task scheduling, and load balancing.

In the context of task scheduling, the Round-Robin algorithm is designed to provide fair and equal access to system resources for multiple processes. It works by assigning a fixed time quantum or time slice to each process in a cyclic manner. Each process is allowed to execute for a specified time quantum, and then it is preempted, allowing the next process in the queue to execute.

In the context of computer networks, the round-robin algorithm divides time for each computer connected to the channel, so each computer can receive **packets** for the amount of time allocated to it in a queue manner. 

The algorithm operates based on a circular queue or a ready queue, where processes are placed in a particular order. When a process has completed its time quantum, it is moved to the end of the queue, and the next process in line gets a chance to execute. This process continues until all processes have completed their execution or until a specific termination condition is met.