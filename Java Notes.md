<p><a target="_blank" href="https://app.eraser.io/workspace/86tPDFYMEndkYOwcNJ2q" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>





## Java Multithreading
**1. Core Concepts**

- **Program:** A program is essentially a static set of instructions saved on a disk (like a Java class file). It is not active until a user or system initiates its execution.
- **Process:** When you execute a program, the operating system loads it into RAM. This active instance of the program is called a process. A process contains its own dedicated memory space, resources, and at least one thread of execution.
- **Thread:** A thread is the smallest unit of execution that the CPU can handle independently. Often described as a "lightweight process," threads exist within a process and share the process's resources while maintaining their own execution state.
**2. Memory Architecture in Java**

When a Java application runs, the Java Virtual Machine (JVM) manages memory organization within the process:

- **Heap Memory:** This is the primary shared memory area where objects and data are stored. All threads within a single process share the heap.
- **Method Area:** This area stores class metadata and constant information. Like the heap, it is shared across all threads in the process.
- **Stack Memory:** Unlike the heap, each thread has a private stack. This is where local variables and method execution frames are managed.
- **Program Counter (PC):** Every thread maintains its own program counter, which keeps track of the specific instruction being executed at any given moment.
**3. Execution Mechanics**

- **CPU and Thread Scheduling:** Modern CPUs do not execute processes directly; they schedule and execute threads. Even if you don't explicitly create threads, the JVM always starts a "main thread" to run your code.
- **Context Switching:** In single-core environments, the CPU can only process one thread at a time. To simulate multitasking, the operating system performs context switching—rapidly swapping between threads to give the illusion of simultaneous progress.
- **Concurrent vs. Parallel Execution:**
    - **Concurrent Execution:** Multiple threads are in a state of progress, but because of context switching, the CPU handles them one after another at a high speed.
    - **Parallel Execution:** This requires multi-core CPUs. When multiple cores are available, the system can actually process different threads at the exact same time, achieving true parallelism.

**4. Multitasking vs. Multithreading**

- **Multitasking:** An operating system-level concept where the system runs multiple processes (like a web browser, an IDE, and a music player) at the same time.
- **Multithreading:** A programming-level concept focusing on splitting a single process into multiple tasks to improve efficiency and responsiveness, allowing for more granular control over execution.




<!--- Eraser file: https://app.eraser.io/workspace/86tPDFYMEndkYOwcNJ2q --->