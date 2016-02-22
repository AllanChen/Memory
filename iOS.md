
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

//表示是一个同步线程  
dispatch_sync

//表示一个异步线程  
dispatch_async

// 全局队列，一个特殊的并行队列  
dispatch_get_global_queue

// 主队列，在主线程中运行，因为主线程只有一个，所以这是一个特殊的串行队列
dispatch_get_main_queue

// 从DISPATCH_QUEUE_SERIAL看出，这是串行队列
dispatch_queue_create("com.demo.serialQueue", DISPATCH_QUEUE_SERIAL)

// 同理，这是一个并行队列  
dispatch_queue_create("com.demo.concurrentQueue", DISPATCH_QUEUE_CONCURRENT)

