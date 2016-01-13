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
- Concurrency VS Parallelism
- Critical Section(临界区)
- Blocking VS Non-Blocking
- Deadlock , Starvation and Livelock

#### 3. Two Laws about parallelism :
