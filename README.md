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
- Synchronous VS Asynchronous
  - Synchronous:
    If an API call is synchronous, it means that code execution will block (or wait) for the API call to return before continuing. This means that until a response is returned by the API, your application will not execute any further, which could be perceived by the user as latency or performance lag in your app.
  - Asynchronous:
    Asynchronous calls do not block (or wait) for the API call to return from the server. Execution continues on in your program, and when the call returns from the server, a "callback" function is executed.

- Concurrency VS Parallelism
- Critical Section(临界区)
- Blocking VS Non-Blocking
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
