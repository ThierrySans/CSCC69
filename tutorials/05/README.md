---
layout: default
permalink: /tutorials/05/
---


1. What is the difference between the code that was used to run programs in project 1 and project 2?  

2. How does a user program (as a file on the disk) become a thread?

3. When you run the `args-none` test, how come the user programs does not print anything?

4. Change the *esp pointer to ignore command line args for now (change line 441 in process.c to `*esp = PHYS_BASE - 12;`) and add an infinite loop to process_wait, what is the output now and why?

5. In the previous question, we saw that a system call occurred. Trace `args.c` and identify how the code reached the `syscall_handler`. 

   1. Which line in `args.c` calls functions that make a syscall?

   2. Where is the code on the user side that invokes the syscall using an interrupt (trap)?

6. Run the args-none user program with GDB and put a breakpoint at `syscall.c` line 18. Continue the code to the breakpoint. Then using the 'x' command in GDB (use `help x` to view manual for the command), identify the items on the stack frame. You should refer to the `write` syscall specification in the project 2 handout.
