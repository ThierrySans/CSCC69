---
layout: default
permalink: /tutorials/03/
---

1. What is a critical section? Can you identify a critical section in the Pintos test `alarm-wait.c`? 

2. What is a mutex (a.k.a lock)?

3. What is a semaphore? How is it different from lock / mutex?

4. Here is a very naive implementation of a lock. Could you explain why disabling the interrupts while holding the lock seems to be a good idea at first? 

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

5. However, could you also also explain why it is actually not a good idea after all?

6. How are locks actually implemented in Pintos?

7. Semaphores operations P and V requires multiple CPU instructions, how does Pintos ensure those operations are atomic?

8. What is a deadlock? Can you give a simple example of a deadlock?