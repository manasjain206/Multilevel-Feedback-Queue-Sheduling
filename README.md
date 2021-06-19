# Multilevel-Feedback-Queue-Sheduling
A CPU scheduler for n number of processes using multilevel feedback queue algorithm. Considering three levels of queue. In first level, RR(tq=2) is used to execute all the processes and in second level, RR(tq=4) is used to execute remaining incomplete processes. If the processes still not complete, these are brought in last level (FCFS) queue.
