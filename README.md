# Operating System Fundamentals for Backend Engineers

A curated list of OS concepts every backend engineer should know, with practical examples in Go.  
*Contribute by adding examples, diagrams, or explanations! [License](LICENSE)*  

---

## Table of Contents

### [1. Process Management](#process-management)
- [Processes vs Threads](#processes-vs-threads)
- [Scheduling](#scheduling)
- [Context Switching](#context-switching)
- [Inter-Process Communication (IPC)](#ipc)
- [Signals](#signals)
- [Daemons](#daemons)

### [2. Memory Management](#memory-management)
- [Virtual Memory](#virtual-memory)
- [Paging & Swapping](#paging-swapping)
- [Memory Allocation](#memory-allocation)
- [Garbage Collection (Go)](#garbage-collection)
- [Memory Leaks](#memory-leaks)

### [3. File Systems](#file-systems)
- [File I/O Operations](#file-io)
- [Permissions & Ownership](#file-permissions)
- [Inodes & Metadata](#inodes)
- [Distributed File Systems](#distributed-fs)

### [4. Networking](#networking)
- [TCP/IP Stack](#tcp-ip)
- [Socket Programming (Go)](#sockets)
- [DNS Resolution](#dns)
- [Load Balancing](#load-balancing)
- [HTTP/HTTPS & gRPC](#http-protocols)

### [5. Concurrency & Parallelism](#concurrency)
- [Goroutines & the Go Scheduler](#goroutines)
- [Mutexes & Atomic Operations](#mutexes)
- [Channels & Patterns](#channels)
- [Race Detection](#race-conditions)

### [6. System Calls](#system-calls)
- [Types of Syscalls](#syscall-types)
- [Syscalls in Go (e.g., `syscall` package)](#go-syscalls)
- [Overhead & Optimization](#syscall-performance)

### [7. Performance Monitoring & Tuning](#performance)
- [Tools: `top`, `vmstat`, `iostat`](#perf-tools)
- [Profiling in Go (`pprof`)](#go-profiling)
- [Benchmarking](#benchmarking)

### [8. Security](#security)
- [User/Kernel Mode & Permissions](#user-kernel-mode)
- [Isolation (cgroups, namespaces)](#isolation)
- [Syscall Filtering (seccomp)](#seccomp)
- [Cryptography (Go `crypto` package)](#crypto)

### [9. Virtualization & Containers](#virtualization)
- [Docker Internals](#docker)
- [Kubernetes & Pods](#kubernetes)
- [cgroups/Namespaces in Go](#cgroups-go)

### [10. Kernel Modules](#kernel-modules)
- [Writing a Simple Module](#kernel-module-basics)
- [Interacting with Hardware](#kernel-hardware)

---

## Detailed Topics & Examples

### 1. Process Management <a name="process-management"></a>
#### Processes vs Threads <a name="processes-vs-threads"></a>
- **Explanation**: Differences in memory sharing, lifecycle, and use cases.
- **Go Example**: Launching processes with `exec.Command`, threads via goroutines.

#### Scheduling <a name="scheduling"></a>
- **Explanation**: Preemptive vs cooperative scheduling.
- **Go Example**: The Go runtime scheduler (M:N scheduling).

---

*(Continue expanding each section with explanations, diagrams, and Go snippets!)*

---

## Contributing
Found a typo? Have a better example? Open a PR! See [CONTRIBUTING.md](CONTRIBUTING.md).

## License
[MIT](LICENSE)
