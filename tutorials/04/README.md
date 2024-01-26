---
layout: default
permalink: /tutorials/04/
---


1. What is the current scheduling strategy used by Pintos? Where in the code is this strategy implemented?

2. As defined in the structure `thread` (in `thread.h` line 83), each thread has a priority. How this priority used by the current scheduling strategy?

3. How many priority levels are there? Which one is the lowest priority and which one is the higher? 

4. Considering 3 threads: `H` (high Priority), `M` (medium priority) and `L` (low priority), can you explain a situation where the thread H would starve (meaning not get the CPU) despite its high priority? 

5. What is the technique to solve this problem? 

6. (Simple donation) What should line `priority_donate_one.c:35` print out and why? 

7. (Simple donation) After we release the lock in `priority_donate_one.c:40`, which thread should get the lock and what the priority of the main thread should be lowered to?

8. (Multiple donations) What should line `priority_donate_multiple.c:39` and line `42` print out and why? 

9. (Multiple donations) What should line `priority_donate_multiple.c:48` print out and why? 
