---
layout: default
permalink: /tutorials/02/
---

After tracing few examples in the debugger, you should be able to understand how Pintos manages threads. Here are few questions to test your understanding: 

1. What variable stores all information about the threads? Where is it defined in the code?

2. When are the different thread created? 

3. What are the different status of a thread?

4. When you print the stack in gdb (using the command `backtrace` or `bt`), the stack shown belongs to which thread? 

5. When the scheduler is called (function `schedule`, line 553 in `thread.c`), how is the next thread selected?

6. When (i.e where in the code) is the scheduler called:

7. Could you give two situations when `thread yield` is called:

8. When the scheduler switches to the next thread, can you precisely locate in the code where the current instruction pointer (eip) and stack pointer (esp) are recorded and replaced by the ones for the next thread? 

9. When the CPU receives an interrupt, can you precisely locate in the code where the current current instruction pointer (eip) and stack pointer (esp) are saved and later restored? 

10. When the CPU receives an interrupt, how does the interrupt handler knows which interrupt has been triggered? 
