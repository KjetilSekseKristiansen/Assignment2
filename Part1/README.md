# Mutex and Channel basics

### What is an atomic operation?
> Atomic operations in concurrent programming are program operations that run completely independently of any other processes. 

### What is a semaphore?
> An abstract data type used to control access to a common resource by multiple processes in a concurrent system. 

### What is a mutex?
> When I am having a big heated discussion at work, I use a rubber chicken which I keep in my desk for just such occasions. The person holding the chicken is the only person who is allowed to talk. If you don't hold the chicken you cannot speak. You can only indicate that you want the chicken and wait until you get it before you speak. Once you have finished speaking, you can hand the chicken back to the moderator who will hand it to the next person to speak. This ensures that people do not speak over each other, and also have their own space to talk.

Replace Chicken with Mutex and person with thread and you basically have the concept of a mutex

### What is the difference between a mutex and a binary semaphore?
> *Your answer here*

### What is a critical section?
> *Your answer here*

### What is the difference between race conditions and data races?
 > Race condition: A race condition is a situation, in which the result of an operation depends on the interleaving of certain individual operations.

Data race: A data race is a situation, in which at least two threads access a shared variable at the same time. At least on thread tries to modify the variable.

### List some advantages of using message passing over lock-based synchronization primitives.
> Message passing is useful for exchanging smaller amounts of data, because no conflicts need be avoided. It's much easier to implement than is shared memory for intercomputer communication. Also, message passing has the advantage that application developers don't need to worry about the details of protections like shared memory.

### List some advantages of using lock-based synchronization primitives over message passing.
> Lock-based synchronization primitives allows maximum speed and convenience of communication, as it can be done at memory speeds when within a computer. It is usually faster than message passing, as message-passing are typically implemented using system calls and thus require the more time-consuming tasks of kernel intervention. In contrast, in shared-memory systems, system calls are required only to establish shared-memory regions. Once established, all access are treated as normal memory accesses w/o extra assistance from the kernel.
