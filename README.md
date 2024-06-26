# Modern C++ concurrency lib minimum tutorial  
This is the road that I learn about c++ concurrency. There may be some mistakes, you can contact me through email(q0r1y@outlook.com) or issue.
## Intro
Modern C++ includes built-in support for:
- [Thread](#thread)
- [Atomic](#atomic)
- [Mutex](#mutex)
- [Condition variable](#condition-variable)
- [Future](#future)

It's confuse when you see these classes, and I will write this note to record my learning process.  
(This is a simple tutorial for modern c++ beginner.)

## [Thread](thread/README.md#thread)
[Thread](https://en.wikipedia.org/wiki/Thread_(computing)) is the base of concurrency. Threads allow multiple functions to execute concurrently.  
- [thread](thread/README.md#stdthread)  
- [jthread](thread/README.md#stdjthread)  

## [Atomic](atomic/README.md#atomic)
- [atomic](atomic/README.md#stdatomic)  

## [Lock](lock/README.md#lock)  
You know something about POSIX lock API such as `pthread_mutex_init()`, `pthread_mutex_lock()`, `pthread_mutex_unlock()`.  
The class `std::mutex` encapsulate pthread lock lib.
- [mutex](lock/README.md#stdmutex)  

The class `std::lock_guard` is a mutex wrapper that provides a convenient RAII-style mechanism for owning a mutex for the duration of a scoped block.
- [lock_guard](lock/README.md#stdlock_guard)  

The use of `std::unique_lock` is similar to `std::mutex`.  
- [unique_lock](lock/README.md#stdunique_lock)

## [Condition variable](condition_variable/README.md#condition-variable)  
A condition variable is an object able to block the calling thread until notified to resume.

## [Future](future/README.md)  
Here is something you need to transfer value between threads.  
- [future](future/README.md#stdfuture)
- [async](future/README.md#stdasync)
- [promise](future/README.md#stdpromise)
- [packaged_task](future/README.md#stdpackaged_task)

## Reference
- [cppreference](https://en.cppreference.com/w/cpp/thread)
- [Bo Qian's Youtube video](https://www.youtube.com/@BoQianTheProgrammer)