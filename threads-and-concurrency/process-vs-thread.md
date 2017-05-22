## Process VS Thread

![](/assets/process_vs_thread.png)

PCB = Process Control Block

#### Process

Single process:

__1.Address space__

Represented by it's addr space:
-Virtual->physical addr mappings(code,data,files)

__2.Execution context__

Represented by it's execution context:
-Values of registers
-Stack pointers, program content

__3.All in a PCB (process control block)__

#### Thread

__1.Address space__

Same virtual addr space
-Share all virtual->physical mappings (all code,data,files)

__2.Execution context__

Multiple independent execution contexts
-Diff instructions, diff input/output
-Access diff portion of addr space

Each thread
-Diff registers, stack pointers

__3.PCB (process control block)__

-Shared part among threads
-Pre-thread exec context