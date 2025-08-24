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
  - Security & Access Control: Protects against unauthorized access and ensures user data privacy.

## Process, Program, and Thread

### Process:
  - A process is a program that is currently being executed by the operating system. It is not just the code, but also includes the program’s current activity, state, memory layout, allocated                         resources, and data needed during execution.
    
### Types of Processes
  **System Processes** are core processes created and managed by the operating system to perform essential system-level tasks.

  - **Characteristics**:
    - Handle critical operations like memory management, device drivers, and background services.
    - Typically run with higher privileges than user processes.
    - Essential for system stability and functionality.
  - **Example**: Kernel processes, task schedulers, or device driver services in Windows or Linux.
  
  **User Processes** are processes initiated by the user through direct actions, such as launching an application.
  
  - **Characteristics**:
    - Started by user interaction (e.g., clicking an application icon).
    - Typically associated with user-level applications.
  - **Example**: Opening a text editor like Notepad or VS Code creates a user process.
  
  ## Foreground Processes
  
  **Foreground Processes** are visible processes that require and involve user interaction, typically tied to applications the user is actively working with.
  
  - **Characteristics**:
    - Directly interact with the user through a graphical or command-line interface.
    - High priority for user responsiveness.
  - **Example**: A word processor (e.g., Microsoft Word) or a web browser actively in use.
  
  ## Background Processes
  
  **Background Processes** run without direct user interaction, performing tasks silently in the background.
  
  - **Characteristics**:
    - Operate independently of user input.
    - Often handle system or application maintenance tasks.
  - **Example**: File synchronization tools (e.g., Dropbox) or system update services.

### Program: 
  - A program is a static set of instructions written in a programming language, stored on a disk or other storage medium. It is a passive entity that only defines what the computer is supposed to do.                 It becomes an active process only when the OS loads and executes it.
    
### Thread: 
  - A thread is the smallest unit of execution within a process. If a process is a large task, then threads are the smaller subtasks within it. A process can have one or multiple threads. Each thread                 represents a single sequence of instructions executed independently.
    
### Need / Use of Threads

Threads are used to improve the performance, responsiveness, and efficiency of applications. They are an essential part of modern OS and software design for the following reasons:

  - **Parallel Execution**: Threads allow multiple parts of a program to run at the same time. On multi-core processors, different threads can execute truly in parallel, speeding up performance.
  - **Responsiveness**: In graphical applications, threads ensure smooth user experiences. For instance, one thread can handle user inputs, while others perform background operations like file loading or computations.
  - **Efficient Resource Use**: Creating a thread is faster and consumes fewer system resources compared to creating a new process. Threads within the same process share data easily and communicate without needing inter-process communication mechanisms.

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
