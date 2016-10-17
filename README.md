# PriorityScheduling

1.In priority scheduling algorithm each process has a priority associated with it 
and as each process hits the queue, it is stored in based on its priority so 
that process with higher priority are dealt with first.

2.To prevent high priority processes from running indefinitely the scheduler may 
decrease the priority of the currently running process at each clock tick (i.e., at each clock interrupt).
If this action causes its priority to drop below that of the next highest process, a process switch occurs. 
Alternatively, each process may be assigned a maximum time quantum that it is allowed to run.
When this quantum is used up, the next highest priority process is given a chance to run

Priority scheduling can be either preemptive or non preemptive

A preemptive priority algorithm will preemptive the CPU if the priority of the newly arrival process is
higher than the priority of the currently running process.
A non-preemptive priority algorithm will simply put the new process at the head of the ready queue.
A major problem with priority scheduling is indefinite blocking or starvation. 
A solution to the problem of indefinite blockage of the low-priority process is aging.
Aging is a technique of gradually increasing the priority of processes that wait in the system for a long period of time.

 
Refer C++ code for priority scheduling.
