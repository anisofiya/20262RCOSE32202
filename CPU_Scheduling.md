- CPU scheduling determines which ready process should use the CPU next
- Goal : Maximize CPU utilization and minimize CPU idle time
- Preemptive: OS can interrupt running process to schedule another
- Non-preemptive : running process keeps CPU until it finishes or blocks

Scheduling Algorithms :

- FCFS : Execute in arrival order
- SJF : Select process with shortest CPU burst first
- Priority Scheduling : Select process based on priority
- Round Robin : Allocate fixed time quantum to each process
- Multilevel Queue : Use multiple ready queues with different scheduling policies
- Multilevel Feedback Queue : Allow processes to move between queues based on their behavior and scheduling rules.
