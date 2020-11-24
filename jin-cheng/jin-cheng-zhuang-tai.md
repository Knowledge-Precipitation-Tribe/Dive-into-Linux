# 进程状态

| 状态 | 说明 |
| :--- | :--- |
| R | running or runnable \(on run queue\) 正在执行或者可执行，此时进程位于执行队列中。 |
| D | uninterruptible sleep \(usually I/O\) 不可中断阻塞，通常为 IO 阻塞。 |
| S | interruptible sleep \(waiting for an event to complete\) 可中断阻塞，此时进程正在等待某个事件完成。 |
| Z | zombie \(terminated but not reaped by its parent\) 僵死，进程已经终止但是尚未被其父进程获取信息。 |
| T | stopped \(either by a job control signal or because it is being traced\) 结束，进程既可以被作业控制信号结束，也可能是正在被追踪。 |

