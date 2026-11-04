Process

- A process is a program in execution, identified by a process ID (PID).
- OS stores process information (e.g.: process state, program counter and CPU registers) in a Process Control Block (PCB).
- PCB information is maintained in kernel memory.

Process States :

- New : process newly created
- Ready : waiting to be assigned to CPU
- Running : currently executing in CPU
- Waiting : wait for event such as I/O completion
- Terminated : finished execution

Context Switching

- The OS saves the execution state of the old process and restores the state of the new process using their PCBs.
- can occur when time quantum expires, a process blocks for I/O or a higher priority process becomes ready.
- Disadvantage : saving and restoring process states introduce CPU overhead

Process APIs :

- fork() : create child process
- exec() : replace current process program with a new program
