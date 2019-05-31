# Answers

1. List all of the main states a process may be in at any point in time on a standard Unix system. Briefly explain what each of these states means.

   - New - The process is being created and awaits ready state.
   - Ready - The process is loaded to memory and awaits execution by the processor
   - Running - The instructions are being executed. The are two execution modes: user or kernel
   - Blocked - The process is blocked when it cannot continue without an external change in state or event occurring.
   - Terminated - The process has finished execution.

2. What is a zombie process?

   - Zombie processes are terminated process that haven't been properly trash collected. The instructions are still in memory.

3. How does a zombie process get created? How does one get destroyed?

   - It is created when a child process isn't terminated by its parent process. It is destroyed when the parent process execute the `wait()` system call. After `wait()` is called, the zombie process is completely removed from memory.

4. What are some of the benefits of working in a compiled language versus a non-compiled language? More specifically, what benefits are there to be had from taking the extra time to compile our code?

   - Faster execution and performance.
   - More customization possible.
