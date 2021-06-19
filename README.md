# Multilevel-Feedback-Queue-Algorithm

This Multi-level feedback queue C program consists of 3 linear queues, i.e., Q1, Q2, and Q3.

Q1 is round robin with time quantum 2(RR2),
Q2 is round robin with time quantum 4(RR4), and
Q3 follows first come first serve (FCFS)
The process cannot be executed in the lower queue if there are any jobs in all higher queues. 

A new process enters queue Q1 which is served RR2 When it gains CPU, a process receives 2 milliseconds.
• If it does not finish in 2 milliseconds, the process is moved to queue Q2.
• At Q2 process is again served RR4 and receives 4 additional milliseconds. 
• If it still does not complete, it is pre-empted and moved to queue Q3.
• At Q3 process is executed by first come first serve.
• If it still does not complete, it is processed at Q2 until completed.
 
ADVANTAGES of Multilevel Feedback Queue Scheduling:
1.It is more flexible.
2.It allows different processes to move between different queues.
3.It prevents starvation by moving a process that waits too long for lower priority queue to the higher priority queue.

OUTPUT: The remaining time of processes in each queue level, total waiting time and total turnaround time are displayed.

![image](https://user-images.githubusercontent.com/86141357/122634145-2d93e280-d0fa-11eb-8bac-a0ae4098f192.png)

![image](https://user-images.githubusercontent.com/86141357/122634297-0093ff80-d0fb-11eb-965e-a9b45bbaa52f.png)
