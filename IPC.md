- Allow communication between processes while maintaining memory protection
- Processes normally have separate address spaces and cannot directly access each other's memory

IPC mechanisms : 

- Shared memory : Processes share a memory region and communicate directly not involving kernel. Synchronization (mutex) needed.
- Message Passing : Use send() and receive() operations often through kernel.
- Signals : Notify processes when an event occurs.
- Pipe : Allow one-way data communication between processes.
- Message Queue : Store messages until they can be received.
- Socket : Provide communication endpoint.
