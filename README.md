# JavaHighConcurrency
by tianhang
## Week 1
#### 1. Why we need parallelism ?

- The End of Moore's Law（摩尔定律失效）
- Business needs （业务需要）
  - not only to improve the performace of system , but also sometimes we need multiple processing unit in some specific bussinesses.
  - for example the HTTP server , it creates a Socket for every processing Thread which allows different threads to handle different tasks.
  - Simplify the task scheduling .
  
#### 2. Some important concepts :
- Synchronous VS Asynchronous（mainly aimed at calling method 主要针对方法调用）
  - Synchronous:
    If an API call is synchronous, it means that code execution will block (or wait) for the API call to return before continuing. This means that until a response is returned by the API, your application will not execute any further, which could be perceived by the user as latency or performance lag in your app.
  - Asynchronous:
    Asynchronous calls do not block (or wait) for the API call to return from the server. Execution continues on in your program, and when the call returns from the server, a "callback" function is executed.

- Concurrency VS Parallelism
  - Parallelism : This requires hardware with multiple processing units .(并行需要多核处理器)
  - Concurrency can be implemented and is used a lot on single processing units, nonetheless it may benefit from multiple processing units with respect to speed. 
  
- Critical Section(临界区)
  - In concurrent programming, a critical section is a part of a multi-process program that may not be concurrently executed by more than one of the program's processes. In other words, it is a piece of a program that requires mutual exclusion of access. Typically, the critical section accesses a shared resource, such as a data structure, a peripheral device, or a network connection, that does not allow multiple concurrent accesses.
  
- Blocking VS Non-Blocking（usually，they are used to describe the interaction among multiple threads线程间相互影响）
  - Blocking : Do not allow multiple threads to  access the critical section simultaneously 
  - Non-Blocking : Allow multiple threads to access the critical section simultaneously.

- Deadlock(锁) , Starvation(饥饿) and Livelock(死锁)
- The level of parallelism
  - Blocking
  - Non-Blocking
    - Obstruction-Free(无障碍)
    - Lock-Free(无锁)
    - Wait-Free(无等待)

#### 3. Two Laws about parallelism 
- Amdahl Law
- Gustafson Law
