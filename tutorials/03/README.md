---
layout: default
permalink: /tutorials/03/
---

1. What is a critical section? Can you identify a critical section in the Pintos test `threads/alarm-wait.c`? 

2. Could you explain in details how this critical section could lead to a race condition bug and how that bug would affect the value of the variable `output_pos`? 

3. What is a mutex (a.k.a lock)?

4. What is a semaphore? How is it different from lock / mutex?

5. In the test `threads/priority-sema.c`, there are 10 threads executed in parallel (11 if you count the main thread). Could you give three scenarios of execution in which the maximum value of the semaphore is either 1, 2 or 10?  

6. Here is a very naive implementation of a lock. Could you explain why disabling the interrupts while holding the lock seems to be a good idea at first? 

```
struct lock { 
} 

void acquire (lock) { 
    disable_interrupts();
} 

void release (lock) { 
    enable_interrupts(); 
}
```

7. However, could you also also explain why it is actually not a good idea after all?

8. How are locks actually implemented in Pintos?

9. Semaphores operations P and V requires multiple CPU instructions, how does Pintos ensure those operations are atomic?

10. What is a deadlock? Can you give a simple example of a deadlock?