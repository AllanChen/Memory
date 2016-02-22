
# iOS GCD 名词解析:



**串行和并行都是相对于队列而言的 -队列（负责调度任务）
**

串行队列：一个接一个的调度任务

并发队列：可以同时调度多个任务

Serial Dispatch Queue，这叫做串行队列

Concurrent Dispatch Queue，叫做并行队列

---
dispatch_sync表示是一个同步线程

dispatch_get_main_queue表示运行在主线程中的主队列
