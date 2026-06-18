# 🏛️ Software Design & Architecture

> From OOP principles to system architecture. The art of structuring code that survives change.

---

## 📌 The Design Hierarchy

```
Principles (SOLID, DRY, KISS)
    ↓
Paradigms (OOP, Functional, Procedural)
    ↓
Design Patterns (GoF, Enterprise, Concurrency)
    ↓
Architecture Patterns (Layered, Hexagonal, Event-Driven)
    ↓
System Architecture (Monolith, Microservices, Distributed)
    ↓
Diagrams & Documentation (UML, C4, ADRs)
```

---

## 🧱 Core Principles

### SOLID

| Principle | Meaning | Resource |
|-----------|---------|----------|
| **S** Single Responsibility | One class, one reason to change | [YouTube](https://www.youtube.com/results?search_query=solid+single+responsibility+principle) |
| **O** Open/Closed | Open for extension, closed for modification | [YouTube](https://www.youtube.com/results?search_query=solid+open+closed+principle) |
| **L** Liskov Substitution | Subtypes must be substitutable for base types | [YouTube](https://www.youtube.com/results?search_query=liskov+substitution+principle) |
| **I** Interface Segregation | Many specific interfaces > one general interface | [YouTube](https://www.youtube.com/results?search_query=interface+segregation+principle) |
| **D** Dependency Inversion | Depend on abstractions, not concretions | [YouTube](https://www.youtube.com/results?search_query=dependency+inversion+principle) |

### Other Principles

| Principle | Meaning |
|-----------|---------|
| DRY | Don't Repeat Yourself |
| KISS | Keep It Simple, Stupid |
| YAGNI | You Aren't Gonna Need It |
| Composition over Inheritance | Prefer has-a over is-a |
| Separation of Concerns | Each module handles one concern |
| Law of Demeter | Talk only to immediate friends |
| Principle of Least Surprise | Code should do what the reader expects |
| Tell, Don't Ask | Tell objects what to do, don't query and decide |

### Resources

| Resource | Link |
|----------|------|
| Clean Code (Uncle Bob talks) | [YouTube](https://www.youtube.com/results?search_query=robert+martin+clean+code+lecture) |
| Clean Architecture (Uncle Bob) | [YouTube](https://www.youtube.com/results?search_query=robert+martin+clean+architecture) |
| SOLID Principles (NPTEL) | [NPTEL Software Engineering](https://nptel.ac.in/courses/106105182) |

---

## 🧬 Programming Paradigms

### Object-Oriented Programming (OOP)

| Concept | What |
|---------|------|
| Encapsulation | Bundle data + behavior, hide internals |
| Inheritance | Reuse via parent-child relationships |
| Polymorphism | Same interface, different implementations |
| Abstraction | Expose what, hide how |

| Course | Platform | Link |
|--------|----------|------|
| OOP in Java (NPTEL) | NPTEL (IIT Kharagpur) | [NPTEL](https://nptel.ac.in/courses/106105191) |
| OOP in C++ (NPTEL) | NPTEL (IIT Kharagpur) | [NPTEL](https://nptel.ac.in/courses/106105151) |
| OOP Design (MIT OCW) | MIT | [MIT OCW](https://ocw.mit.edu/courses/6-170-software-studio-spring-2013/) |

### Functional Programming

| Concept | What |
|---------|------|
| Pure Functions | No side effects, same input → same output |
| Immutability | Data never changes after creation |
| Higher-Order Functions | Functions that take/return functions |
| Composition | Build complex from simple functions |
| Monads | Chainable computation contexts |

| Course | Platform | Link |
|--------|----------|------|
| Functional Programming (Haskell) | edX (audit) | [edX](https://www.edx.org/learn/haskell/university-of-glasgow-functional-programming-in-haskell) |
| Category Theory for Programmers | YouTube (Bartosz Milewski) | [YouTube](https://www.youtube.com/playlist?list=PLbgaMIhjbmEnaH_LTkxLI7FMa2HsnawM_) |
| Functional Programming in Scala | Coursera (audit) | [Coursera](https://www.coursera.org/specializations/scala) |

### Other Paradigms

| Paradigm | Use Case | Language Examples |
|----------|----------|-----------------|
| Procedural | Scripts, embedded, OS | C, Bash, Fortran |
| Declarative | Config, queries, UI | SQL, HTML, Terraform |
| Reactive | Event streams, UI | RxJS, Reactor, Akka |
| Actor Model | Concurrency, distributed | Erlang, Akka, Go (goroutines) |
| Data-Oriented | Performance-critical, games | C, C++ (ECS pattern) |
| Logic | AI, constraint solving | Prolog |

---

## 🎨 Design Patterns

### GoF (Gang of Four) 23 Classic Patterns

**Free reference**: [refactoring.guru/design-patterns](https://refactoring.guru/design-patterns)

#### Creational (Object Creation)

| Pattern | When | Example |
|---------|------|---------|
| Singleton | One instance globally | Logger, Config |
| Factory Method | Delegate creation to subclasses | UI widget factories |
| Abstract Factory | Families of related objects | Cross-platform UI |
| Builder | Complex object construction | Query builders, configs |
| Prototype | Clone existing objects | Game entity spawning |

#### Structural (Composition)

| Pattern | When | Example |
|---------|------|---------|
| Adapter | Incompatible interfaces | Legacy API wrappers |
| Bridge | Separate abstraction from implementation | Platform-independent rendering |
| Composite | Tree structures | File systems, UI components |
| Decorator | Add behavior dynamically | Middleware, logging wrappers |
| Facade | Simplify complex subsystems | SDK wrappers |
| Flyweight | Share common state | Text rendering, game tiles |
| Proxy | Control access | Lazy loading, caching, auth |

#### Behavioral (Communication)

| Pattern | When | Example |
|---------|------|---------|
| Observer | Event notification | Pub/sub, UI events |
| Strategy | Interchangeable algorithms | Sorting, compression |
| Command | Encapsulate actions | Undo/redo, task queues |
| State | Object behavior changes with state | TCP connection states |
| Template Method | Algorithm skeleton with hooks | Framework lifecycle |
| Iterator | Sequential access | Collections, streams |
| Chain of Responsibility | Pass request along handlers | Middleware pipelines |
| Mediator | Centralize communication | Chat rooms, event buses |
| Visitor | Add operations without modifying classes | AST traversal, serialization |

### Concurrency Patterns

| Pattern | What | Use Case |
|---------|------|----------|
| Producer-Consumer | Queue between threads | Task processing |
| Thread Pool | Reuse threads | Web servers |
| Future/Promise | Async result placeholder | API calls |
| Actor Model | Message-passing concurrency | Distributed systems |
| Monitor | Mutual exclusion + condition vars | Shared resources |
| Read-Write Lock | Multiple readers, single writer | Caches, databases |
| Barrier | Synchronize thread groups | Parallel computation |
| Double-Checked Locking | Lazy init in multithreaded | Singleton |

### Enterprise Patterns

| Pattern | What | Link |
|---------|------|------|
| Repository | Abstract data access | [martinfowler.com](https://martinfowler.com/eaaCatalog/repository.html) |
| Unit of Work | Track changes, batch commits | [martinfowler.com](https://martinfowler.com/eaaCatalog/unitOfWork.html) |
| CQRS | Separate read/write models | [martinfowler.com/bliki/CQRS](https://martinfowler.com/bliki/CQRS.html) |
| Event Sourcing | Store events, not state | [eventstore.com](https://www.eventstore.com/event-sourcing) |
| Saga | Distributed transactions | [microservices.io/patterns/saga](https://microservices.io/patterns/data/saga.html) |
| Circuit Breaker | Fail fast on downstream failure | [martinfowler.com](https://martinfowler.com/bliki/CircuitBreaker.html) |
| Bulkhead | Isolate failures | [docs.microsoft.com](https://learn.microsoft.com/en-us/azure/architecture/patterns/bulkhead) |

### Resources

| Resource | Link |
|----------|------|
| Refactoring Guru (visual, free) | [refactoring.guru](https://refactoring.guru/design-patterns) |
| Head First Design Patterns (talks) | [YouTube](https://www.youtube.com/results?search_query=head+first+design+patterns) |
| Game Programming Patterns (free book) | [gameprogrammingpatterns.com](https://gameprogrammingpatterns.com/) |
| Christopher Okhravi (YouTube) | [youtube.com/@ChristopherOkhravi](https://www.youtube.com/@ChristopherOkhravi) |
| Derek Banas (YouTube) | [youtube.com/@deaborrekbanas](https://www.youtube.com/@derekbanas) |

---

## 🏗️ Architecture Patterns

### Application Architecture

| Pattern | When | Diagram |
|---------|------|---------|
| **Layered (N-Tier)** | Traditional web apps | Presentation → Business → Data |
| **Hexagonal (Ports & Adapters)** | Testable, framework-independent | Core ← Ports → Adapters |
| **Clean Architecture** | Domain-centric, dependency inversion | Entities → Use Cases → Interface Adapters → Frameworks |
| **Onion Architecture** | Similar to Clean, .NET world | Domain → Application → Infrastructure |
| **Vertical Slice** | Feature-based organization | Each feature owns its full stack |
| **Event-Driven** | Async, decoupled systems | Events → Handlers → Side Effects |
| **Pipe and Filter** | Data transformation pipelines | Input → Filter₁ → Filter₂ → Output |
| **Microkernel (Plugin)** | Extensible systems | Core + Plugins |

### System Architecture

| Pattern | Scale | Use Case |
|---------|-------|----------|
| **Monolith** | Small-medium | Start here. Always. |
| **Modular Monolith** | Medium | Monolith with clear boundaries |
| **Microservices** | Large, multiple teams | Independent deployment |
| **Service Mesh** | Microservices at scale | Istio, Linkerd |
| **Serverless** | Event-driven, variable load | AWS Lambda, Cloud Functions |
| **Edge Computing** | Low latency, IoT | Cloudflare Workers, Fly.io |
| **CQRS + Event Sourcing** | Complex domains | Finance, audit trails |

### Resources

| Resource | Link |
|----------|------|
| Martin Fowler (Architecture) | [martinfowler.com/architecture](https://martinfowler.com/architecture/) |
| Microsoft Azure Architecture Center | [learn.microsoft.com/azure/architecture](https://learn.microsoft.com/en-us/azure/architecture/) |
| Microservices.io (Chris Richardson) | [microservices.io](https://microservices.io/) |
| Clean Architecture (Uncle Bob talk) | [YouTube](https://www.youtube.com/results?search_query=robert+martin+clean+architecture) |
| Hexagonal Architecture (Alistair Cockburn) | [alistair.cockburn.us](https://alistair.cockburn.us/hexagonal-architecture/) |
| Software Architecture Monday (Mark Richards) | [youtube.com/@markrichards5014](https://www.youtube.com/@markrichards5014) |

---

## 📐 Diagrams & Documentation

### Diagram Types

| Diagram | Purpose | Tool |
|---------|---------|------|
| **C4 Model** | System context → Container → Component → Code | [c4model.com](https://c4model.com/) |
| **UML Class Diagram** | Static structure (classes, relationships) | [PlantUML](https://plantuml.com/) |
| **UML Sequence Diagram** | Interaction over time | [Mermaid](https://mermaid.js.org/) |
| **UML Activity Diagram** | Workflow/process flow | [draw.io](https://app.diagrams.net/) |
| **Entity-Relationship (ER)** | Database schema | [dbdiagram.io](https://dbdiagram.io/) |
| **Data Flow Diagram (DFD)** | How data moves through system | [draw.io](https://app.diagrams.net/) |
| **Architecture Decision Record** | Why decisions were made | [adr.github.io](https://adr.github.io/) |

### Diagramming Tools (Free)

| Tool | Best For | Link |
|------|----------|------|
| Mermaid | Diagrams as code (in Markdown) | [mermaid.js.org](https://mermaid.js.org/) |
| PlantUML | UML from text | [plantuml.com](https://plantuml.com/) |
| draw.io (diagrams.net) | General diagramming | [app.diagrams.net](https://app.diagrams.net/) |
| Excalidraw | Whiteboard-style | [excalidraw.com](https://excalidraw.com/) |
| D2 | Declarative diagrams | [d2lang.com](https://d2lang.com/) |
| Structurizr | C4 model | [structurizr.com](https://structurizr.com/) |

### From Design to Code

```
1. Requirements (PRD / User Stories)
    ↓
2. System Design (C4 Context + Container diagrams)
    ↓
3. API Contract (OpenAPI / Protobuf)
    ↓
4. Data Model (ER diagram → migrations)
    ↓
5. Component Design (Class/Sequence diagrams)
    ↓
6. Implementation (TDD: test → code → refactor)
    ↓
7. Review (ADR for decisions, PR for code)
```

---

## 📖 Books

| Book | Free? | Link |
|------|-------|------|
| Refactoring Guru (Patterns) | ✅ | [refactoring.guru](https://refactoring.guru/) |
| Game Programming Patterns | ✅ | [gameprogrammingpatterns.com](https://gameprogrammingpatterns.com/) |
| Architecture of Open Source Apps | ✅ | [aosabook.org](https://aosabook.org/en/) |
| Clean Code (talks) | ✅ (talks) | [YouTube](https://www.youtube.com/results?search_query=robert+martin+clean+code) |
| Domain-Driven Design (talks) | ✅ (talks) | [youtube.com/@ddd_eu](https://www.youtube.com/@ddd_eu) |
| Patterns of Enterprise Application Architecture | ❌ | [martinfowler.com/eaaCatalog](https://martinfowler.com/eaaCatalog/) (catalog free) |
| Design Patterns (GoF) | ❌ | [refactoring.guru](https://refactoring.guru/) (explanations free) |

---
*Cross-references: [Best Practices](best-practices.md) · [Systems Track](../tracks/systems-programming.md) · [Product Engineering](../tracks/product-engineering.md) · [Interview Prep](../tracks/interview-prep.md#-system-design)*
