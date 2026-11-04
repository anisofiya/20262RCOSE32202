1. Monolithic Kernel

   - Most OS components run together in one large kernel.
   - Components can communicate directly without switching address spaces which cause less overhead.
   - One kernel instance exists in memory and is shared by applications.
   - Each process has its own virtual address space but share the same OS kernel.
   - Kernel memory may be mapped into a process virtual address space but user applications cannot directly access protected kernel memory.
   - Advantage : Direct communication (less overhead)
   - Disadvantage : Bug in one kernel component may affect or crash entire system.
   
2. Microkernel
   
   - Only essential functions run in kernel mode such as basic scheduling, IPC, etc.
   - Other OS services such as file systems, device drivers, etc., typically run in user mode.
   - Component communicate through IPC.
   - Advantages: Better isolation, easier to develop and maintain individual services.
   - Disadvantages: Additional IPC and address space switching overhead may reduce performance compared to monolithic kernel.
