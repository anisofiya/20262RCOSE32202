A process can contain multiple threads that execute concurrently. 
Threads within same process share resources such as code, data and heap. 
But each thread has its own program counter, CPU registers and stack. 

Advantages of multithreaded process :

- Parallelism : run a single program with multiple CPU cores in parallel
- Responsiveness : thread can remain active even when another thread is blocked
- Resource sharing : only one memory space between threads
- Economy : reduce overheads in context switching and creating new execution flows

Thread management :

- User-level : managed by a user-level thread library without requiring the kernel to schedule each thread individually
- Kernel-level : kernel schedules a time slice for a thread
