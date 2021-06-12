# Project
thread-safety by semaphore

# OS Environment
Ubuntu 18.04.5

# RESULT

#SEMAPHORE RESULT

![semaphore](https://user-images.githubusercontent.com/84624932/121785928-b6d97f80-cbf7-11eb-9d43-509df45e59cf.png)

#MUTEX RESULT

![tscounter](https://user-images.githubusercontent.com/84624932/121785933-bb9e3380-cbf7-11eb-9209-d28b417f7baa.png)

# Result Analysis
MUTEX is faster than SEMAPHORE
Mutexes are much faster than semaphores because semaphores always require a kernel entry. On most processors, acquisition of a mutex doesn't require entry to the kernel for a free mutex. Since the scope of the semaphore is larger, such as number of counts and waking up of other tasks, the implementation may be little complex and may consume more time than mutex.
(source : http://dtdtech.blogspot.com/2012/01/why-mutex-is-faster-than-semaphore.html)

