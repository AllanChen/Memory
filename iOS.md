
# iOS GCD 名词解析:



**串行和并行都是相对于队列而言的 -队列（负责调度任务）
**

串行队列：一个接一个的调度任务

并发队列：可以同时调度多个任务

Serial Dispatch Queue，这叫做串行队列

Concurrent Dispatch Queue，叫做并行队列

---

**同步与异步**

**串行与并行针对的是队列，而同步与异步，针对的则是线程。** 

dispatch_sync 表示是一个同步线程

dispatch_async 表示一个异步线程

dispatch_get_main_queue 表示运行在主线程中的主队列
