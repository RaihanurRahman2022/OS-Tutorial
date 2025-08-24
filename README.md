# Operating System Fundamentals for Backend Engineers

A curated list of OS concepts every backend engineer should know, with practical examples in Go.  
*Contribute by adding examples, diagrams, or explanations! [License](LICENSE)*  

---

# Table of Contents

### Basics of Operating Systems
- [Operating System Introduction](#operating-system-introduction)
- [Process, Program, and Thread](#process-program-and-thread)
- [Types of Operating Systems](#types-of-operating-systems)
  - [Batch OS](#batch-os)
  - [Multiprogramming OS](#multiprogramming-os)
  - [Multitasking OS](#multitasking-os)
  - [Multiprocessing OS](#multiprocessing-os)
  - [Real-time OS](#real-time-os)
  - [Distributed OS](#distributed-os)
  - [Clustered OS](#clustered-os)
  - [Embedded OS](#embedded-os)
- [Contributing](#contributing)
- [License](#license)

## Operating System Introduction

An **operating system (OS)** is system software that manages computer hardware, software resources, and provides common services for computer programs. It acts as an intermediary between users and computer hardware, ensuring efficient operation and resource allocation.

- **Key Functions**:
  - Process management: Handles creation, scheduling, and termination of processes.
  - Memory management: Allocates and deallocates memory for processes.
  - File system management: Organizes and manages data storage.
  - Device management: Controls hardware devices like printers and disks.
  - User interface: Provides interaction via GUI or command-line interfaces.

## Process, Program, and Thread

- **Program**: A static set of instructions stored on disk (e.g., an executable file).
- **Process**: A program in execution, including its code, data, and system resources like memory and CPU time.
- **Thread**: A smaller unit of execution within a process. Multiple threads within a process share resources but execute independently.

*Example*: A web browser (program) runs as a process, with threads handling tasks like rendering pages and downloading files.

## Types of Operating Systems

### Batch OS

**Batch Operating Systems** process jobs in batches without user interaction. Jobs are collected, grouped, and executed sequentially.

- **Characteristics**:
  - No direct user interaction during execution.
  - Jobs processed in a queue for efficiency.
  - Common in early systems for tasks like payroll or data processing.
- **Example**: IBM OS/360 for batch processing.

### Multiprogramming OS

**Multiprogramming OS** keeps multiple programs in memory, allowing the CPU to switch between them when one is waiting (e.g., for I/O operations).

- **Characteristics**:
  - Multiple programs loaded in memory simultaneously.
  - Improves CPU utilization by reducing idle time.
  - Enhances system throughput.
- **Example**: Early UNIX systems.

### Multitasking OS

**Multitasking OS** allows multiple tasks to run concurrently by rapidly switching between them, providing a seamless user experience.

- **Characteristics**:
  - Supports time-sharing for multiple tasks.
  - Rapid context switching creates the illusion of parallel execution.
  - Ideal for interactive systems like desktops.
- **Example**: Windows, macOS, Linux.

### Multiprocessing OS

**Multiprocessing OS** manages systems with multiple CPUs or cores, enabling true parallel execution of processes.

- **Characteristics**:
  - Distributes tasks across multiple processors.
  - Enhances performance for compute-intensive applications.
  - Requires complex scheduling algorithms.
- **Example**: Modern Linux kernels, Windows Server.

### Real-time OS

**Real-time OS (RTOS)** is designed for systems with strict timing requirements, ensuring immediate response to inputs.

- **Characteristics**:
  - Predictable and low-latency response times.
  - Hard real-time (strict deadlines) or soft real-time (flexible deadlines).
  - Used in critical systems like medical devices or robotics.
- **Example**: VxWorks, RTEMS.

### Distributed OS

**Distributed OS** manages a group of independent computers that work together as a single system, sharing resources transparently.

- **Characteristics**:
  - Runs across networked computers.
  - Provides scalability and fault tolerance.
  - Resources like files and processors are shared.
- **Example**: Amoeba, Plan 9.

### Clustered OS

**Clustered OS** manages a group of computers (nodes) working as a single system for high availability or load balancing.

- **Characteristics**:
  - Ensures high availability and reliability.
  - Balances workloads across nodes.
  - Used in large-scale systems like web servers.
- **Example**: Microsoft Windows HPC Server, Linux-based clusters.

### Embedded OS

**Embedded OS** is designed for resource-constrained devices, such as IoT gadgets, appliances, or automotive systems.

- **Characteristics**:
  - Lightweight and optimized for specific hardware.
  - Minimal resource usage (memory, CPU).
  - Common in consumer electronics and IoT.
- **Example**: FreeRTOS, Embedded Linux.

## Contributing

Feel free to contribute to these notes by submitting pull requests or opening issues for suggestions, corrections, or additional content.

## License

This document is licensed under the [MIT License](LICENSE).
