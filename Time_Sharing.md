Time sharing divides CPU time into small intervals (time quantum). 
It allows multiple programs to share a single CPU core through frequent context switching. 
During context switch, CPU registers and the program counter must be saved and restored. 
Time sharing enables concurrent execution where multiple programs make progress during overlapping periods.
On a single CPU core, programs do not actually execute simultaneously but the CPU switches between them quickly.
However, the frequent context switching introduces overhead and wastes CPU time that could be used for actual execution.
