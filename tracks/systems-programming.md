# ⚙️ Systems Programming Track

> Operating systems, compilers, databases, networking the infrastructure that everything else runs on.

---

## 🎯 Target Roles

- Systems Engineer
- Kernel Developer
- Compiler Engineer
- Database Engineer
- Network Engineer (low-level)
- Performance Engineer
- Infrastructure Engineer (bare-metal)

---

## 📚 Core Courses

### Operating Systems

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Operating Systems (6.828/6.S081)](https://pdos.csail.mit.edu/6.828/) | MIT OCW | MIT | Advanced |
| [Operating Systems](https://nptel.ac.in/courses/106106144) | NPTEL | IIT Madras | Intermediate |
| [Introduction to Operating Systems](https://www.udacity.com/course/introduction-to-operating-systems--ud923) | Udacity (free) | Georgia Tech | Intermediate |
| [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) | Free Book | UW-Madison | Intermediate |
| [Advanced Operating Systems](https://www.udacity.com/course/advanced-operating-systems--ud189) | Udacity (free) | Georgia Tech | Advanced |
| [Linux Kernel Programming](https://nptel.ac.in/courses/106106198) | NPTEL | IIT Bombay | Advanced |

### Compilers & Language Implementation

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Compilers (CS143)](https://www.edx.org/learn/computer-science/stanford-university-compilers) | edX (audit) | Stanford | Intermediate |
| [Compiler Design](https://nptel.ac.in/courses/106104123) | NPTEL | IIT Kanpur | Intermediate |
| [Crafting Interpreters](https://craftinginterpreters.com/) | Free Book | Bob Nystrom | Intermediate |
| [Build Your Own Lisp](https://buildyourownlisp.com/) | Free Book | Daniel Holden | Beginner |
| [LLVM Tutorial](https://llvm.org/docs/tutorial/) | Official Docs | LLVM Project | Advanced |
| [Programming Languages (CS173)](https://www.youtube.com/playlist?list=PLbdXd8eufjyVMm9h-_bBqXMGJ9MXlftY_) | YouTube | Brown University | Intermediate |

### Database Internals

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Database Systems (15-445)](https://15445.courses.cs.cmu.edu/) | YouTube/CMU | CMU (Andy Pavlo) | Intermediate |
| [Advanced Database Systems (15-721)](https://15721.courses.cs.cmu.edu/) | YouTube/CMU | CMU (Andy Pavlo) | Advanced |
| [Database Management Systems](https://nptel.ac.in/courses/106106093) | NPTEL | IIT Madras | Intermediate |
| [Architecture of a Database System](https://dsf.berkeley.edu/papers/fntdb07-architecture.pdf) | Free Paper | UC Berkeley | Advanced |

### Computer Networking (Low-Level)

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Computer Networks](https://nptel.ac.in/courses/106105183) | NPTEL | IIT Kharagpur | Intermediate |
| [Computer Networking (Stanford)](https://www.youtube.com/playlist?list=PLoCMsyE1cvdWKsLVyf6cPwCLDIZnOj0NS) | YouTube | Stanford | Intermediate |
| [Beej's Guide to Network Programming](https://beej.us/guide/bgnet/) | Free Book | Brian Hall | Intermediate |
| [High Performance Browser Networking](https://hpbn.co/) | Free Book | Ilya Grigorik | Advanced |
| [TCP/IP Illustrated (lectures)](https://www.youtube.com/results?search_query=tcp+ip+illustrated+lecture) | YouTube | Various | Advanced |

### Concurrency & Parallel Programming

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Parallel Computer Architecture](https://nptel.ac.in/courses/106102114) | NPTEL | IIT Kanpur | Advanced |
| [Concurrent Programming in Java](https://www.coursera.org/learn/concurrent-programming-in-java) | Coursera (audit) | Rice University | Intermediate |
| [Performance Engineering (6.172)](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/) | MIT OCW | MIT | Advanced |
| [The Art of Multiprocessor Programming](https://www.youtube.com/playlist?list=PL2SOU6wwxB0uP4rJgf5ayhHWgw7akUWSf) | YouTube | Various | Advanced |

### Distributed Systems

| Course | Platform | Institution | Level |
|--------|----------|-------------|-------|
| [Distributed Systems (6.824)](https://pdos.csail.mit.edu/6.824/) | MIT OCW | MIT | Advanced |
| [Distributed Computing](https://nptel.ac.in/courses/106106168) | NPTEL | IIT Patna | Intermediate |
| [Designing Data-Intensive Applications (talks)](https://www.youtube.com/results?search_query=martin+kleppmann+designing+data+intensive) | YouTube | Martin Kleppmann | Advanced |

---

## 🛠️ Practical Projects

| Project | What You Learn | Resource |
|---------|---------------|----------|
| Write a shell | Process management, syscalls | [Build Your Own Shell](https://github.com/tokenrove/build-your-own-shell) |
| Write a malloc | Memory management | [Writing a Memory Allocator](http://dmitrysoshnikov.com/compilers/writing-a-memory-allocator/) |
| Write a TCP stack | Networking from scratch | [Let's Code a TCP/IP Stack](https://www.saminiir.com/lets-code-tcp-ip-stack-1-ethernet-arp/) |
| Write a database | Storage engines, B-trees | [Build Your Own Database](https://build-your-own.org/database/) |
| Write a compiler | Parsing, codegen, optimization | [Crafting Interpreters](https://craftinginterpreters.com/) |
| Write an OS | Everything | [Writing an OS in Rust](https://os.phil-opp.com/) |
| Write a container | Namespaces, cgroups | [Containers from Scratch](https://ericchiang.github.io/post/containers-from-scratch/) |

---

## 📖 Essential Reading (Free)

| Book | Topic | Link |
|------|-------|------|
| OSTEP | Operating Systems | [ostep.org](https://pages.cs.wisc.edu/~remzi/OSTEP/) |
| Dive into Systems | Computer Systems | [diveintosystems.org](https://diveintosystems.org/) |
| Crafting Interpreters | Compilers | [craftinginterpreters.com](https://craftinginterpreters.com/) |
| Beej's Network Guide | Networking | [beej.us/guide/bgnet](https://beej.us/guide/bgnet/) |
| The Architecture of Open Source Applications | System design | [aosabook.org](https://aosabook.org/en/) |
| Database Internals (talks) | Storage engines | [CMU DB YouTube](https://www.youtube.com/@CMUDatabaseGroup) |

---

## 📖 Learning Path

```
Beginner:     C programming → Data structures → Computer architecture
Intermediate: OS concepts → Networking → Concurrency → Build a shell
Advanced:     Kernel hacking → Compiler construction → Database internals
Expert:       Distributed systems → Formal verification → Performance engineering
```

---

*"Systems programming is where you learn that abstractions leak, hardware lies, and the only truth is the assembly output."*
