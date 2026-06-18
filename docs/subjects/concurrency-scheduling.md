# ⚡ Concurrency, Parallelism & Scheduling

> Threads, locks, async, schedulers the hardest problems in computing after naming things.

→ *See also: [OS & Kernel](os-kernel.md) · [Systems Track](../tracks/systems-programming.md) · [C++](../languages/cpp.md)*

---

## 🧵 Concurrency vs Parallelism

```
Concurrency: Dealing with multiple things at once (structure)
Parallelism: Doing multiple things at once (execution)

Concurrency is about composition. Parallelism is about speed.
Rob Pike
```

---

## 📚 Courses

| Course | Platform | Link |
|--------|----------|------|
| Concurrent Programming in Java | Coursera (audit, Rice) | [Coursera](https://www.coursera.org/learn/concurrent-programming-in-java) |
| Parallel Programming in Java | Coursera (audit, Rice) | [Coursera](https://www.coursera.org/learn/parallel-programming-in-java) |
| Performance Engineering (MIT 6.172) | MIT OCW | [MIT OCW](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/) |
| Parallel Computer Architecture (NPTEL) | NPTEL (IIT Kanpur) | [NPTEL](https://nptel.ac.in/courses/106102114) |
| Real-Time Systems (NPTEL) | NPTEL (IIT Kharagpur) | [NPTEL](https://nptel.ac.in/courses/106105036) |
| Concurrency is Not Parallelism (Rob Pike) | YouTube | [YouTube](https://www.youtube.com/watch?v=oV9rvDllKEg) |
| The Art of Multiprocessor Programming (talks) | YouTube | [YouTube](https://www.youtube.com/playlist?list=PL2SOU6wwxB0uP4rJgf5ayhHWgw7akUWSf) |

---

## 🔒 Concurrency Primitives

| Primitive | What | When |
|-----------|------|------|
| Mutex | Mutual exclusion lock | Protect shared state |
| Semaphore | Counting lock | Limit concurrent access |
| Condition Variable | Wait for a condition | Producer-consumer |
| Read-Write Lock | Multiple readers OR one writer | Read-heavy workloads |
| Spinlock | Busy-wait lock | Very short critical sections |
| Atomic Operations | Lock-free single-variable ops | Counters, flags |
| Barrier | Wait for all threads | Parallel phases |
| Channel | Message passing (Go, Rust) | CSP-style concurrency |
| Future/Promise | Async result | Non-blocking I/O |

---

## 🏗️ Concurrency Models

| Model | Language/Runtime | Key Idea |
|-------|-----------------|----------|
| **Threads + Locks** | C, C++, Java | Shared memory, explicit synchronization |
| **CSP (Communicating Sequential Processes)** | Go (goroutines + channels) | Don't share memory; share by communicating |
| **Actor Model** | Erlang, Akka, Elixir | Isolated actors, message passing |
| **Async/Await** | Python, JS, Rust, C# | Cooperative multitasking, event loop |
| **Data Parallelism** | CUDA, OpenMP, SIMD | Same operation on many data points |
| **Fork-Join** | Java ForkJoinPool, Rayon (Rust) | Divide work, join results |
| **Software Transactional Memory** | Haskell, Clojure | Database-like transactions for memory |

---

## 📅 Scheduling

### OS Scheduling Algorithms

| Algorithm | Type | Use Case |
|-----------|------|----------|
| FIFO (First Come First Served) | Non-preemptive | Batch processing |
| Round Robin | Preemptive, time-slice | General-purpose OS |
| Priority Scheduling | Preemptive | Real-time systems |
| Shortest Job First (SJF) | Non-preemptive | Batch optimization |
| Multilevel Feedback Queue | Preemptive, adaptive | Linux CFS inspiration |
| Completely Fair Scheduler (CFS) | Preemptive | Linux default |
| Earliest Deadline First (EDF) | Preemptive | Hard real-time |
| Rate Monotonic (RM) | Static priority | RTOS, periodic tasks |

### Real-Time Scheduling
→ *See [Embedded Track](../tracks/embedded-systems.md)*

| Concept | What |
|---------|------|
| Hard real-time | Missing deadline = system failure |
| Soft real-time | Missing deadline = degraded quality |
| Priority inversion | Low-priority task blocks high-priority |
| Priority inheritance | Temporarily boost blocking task |
| Watchdog timer | Reset if task doesn't complete in time |

### Resources

| Resource | Link |
|----------|------|
| OSTEP: Scheduling chapters | [ostep.org](https://pages.cs.wisc.edu/~remzi/OSTEP/) |
| Linux CFS explained | [kernel.org/doc](https://www.kernel.org/doc/html/latest/scheduler/sched-design-CFS.html) |
| Real-Time Linux | [wiki.linuxfoundation.org/realtime](https://wiki.linuxfoundation.org/realtime/start) |

---

## 🔓 Lock-Free & Wait-Free Programming

| Resource | Link |
|----------|------|
| Herb Sutter: Lock-Free Programming (CppCon) | [YouTube](https://www.youtube.com/watch?v=ZQFzMfHIxng) |
| Jeff Preshing: Lock-Free Blog | [preshing.com](https://preshing.com/) |
| Memory Models (C++ atomics) | [YouTube](https://www.youtube.com/results?search_query=c%2B%2B+memory+model+atomics) |
| Fedor Pikus: C++ Atomics (CppCon) | [YouTube](https://www.youtube.com/results?search_query=fedor+pikus+atomics+cppcon) |

---

## 🐛 Common Concurrency Bugs

| Bug | What | Prevention |
|-----|------|-----------|
| Race Condition | Outcome depends on timing | Locks, atomics, immutability |
| Deadlock | Threads wait for each other forever | Lock ordering, timeouts |
| Livelock | Threads keep retrying, no progress | Backoff strategies |
| Starvation | Thread never gets CPU time | Fair scheduling, priority |
| Priority Inversion | High-priority blocked by low-priority | Priority inheritance |
| ABA Problem | Value changes A→B→A, CAS succeeds incorrectly | Hazard pointers, epoch-based reclamation |

---

## 📖 Books

| Book | Free? | Link |
|------|-------|------|
| The Little Book of Semaphores | ✅ | [greenteapress.com/semaphores](https://greenteapress.com/wp/semaphores/) |
| Is Parallel Programming Hard? | ✅ | [kernel.org/pub/linux/kernel/people/paulmck/perfbook](https://www.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html) |
| OSTEP (Concurrency chapters) | ✅ | [ostep.org](https://pages.cs.wisc.edu/~remzi/OSTEP/) |
| Java Concurrency in Practice | ❌ (talks free) | [YouTube](https://www.youtube.com/results?search_query=java+concurrency+in+practice) |
| C++ Concurrency in Action | ❌ | Reference |
| The Art of Multiprocessor Programming | ❌ (lectures free) | [YouTube](https://www.youtube.com/playlist?list=PL2SOU6wwxB0uP4rJgf5ayhHWgw7akUWSf) |

---
*Cross-references: [OS & Kernel](os-kernel.md) · [C++](../languages/cpp.md) · [Rust](../languages/rust.md) · [Go](../languages/go.md) · [Embedded Track](../tracks/embedded-systems.md)*
