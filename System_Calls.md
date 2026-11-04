System calls provide an interface to enter the kernel mode from user node. 
They allow applications to access protected services provided by kernel. 
Applications usually use high level APIs (e.g.: Standard C library) to invoke system calls.
However, not every API function require system call, such as simple calculations. 
The OS identifies which system call to execute using a system call number and system call table.

System Call Parameter Parsing:

- Registers : fast and simple but limited to number of available registers.
- Pass Metadata: parameters stored in memory and their address is passed to the system call handler.

System Call Handler:

- Identify the system call number
- Execute the corresponding handler
- Check the parameters location (registers or memory)
- Perform the requested operations
- Return results
