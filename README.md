# Linux-kernel-questions
A few question about Linux kernel and tracing tools

*What is interrupts and system calls in OS?*

answer:


1. **System Call**: A system call is a method that enables a user process to interact with the kernel of the operating system¹. It's a call from user mode to kernel mode¹. We can use system calls to read information from files, get time, manage the computer’s memory, or control the data flow between computers¹. A user program initiates a system call by executing an instruction that transfers control from the user program to the operating system kernel¹. System calls can be divided into five categories based on their use: process control, maintenance of information, management of participating devices, handling communication, and file management¹.

2. **System Interrupt**: System interrupts are a way for a process to alert the kernel that an event has occurred¹. Once interrupted, the kernel can process the event and return to the process where it left off¹. An interrupt is an alert triggered by events such as the completion of an instruction, hardware or software signaling for an event, and timers reaching their final countdown value¹. Interrupts can be initiated from software to implement concurrency control mechanisms¹. They can also arise in response to some asynchronous event¹. Interrupts can be divided into two types: software interrupts and hardware interrupts². Software interrupts are produced by software or a system, often to carry out a certain function or respond to an error condition². Hardware interrupts are signals emitted by hardware when a process or an event needs immediate attention².

*State five major differences between interrupts and system calls in Linux operating system*

Sure, here are five major differences between system calls and interrupts in the Linux operating system:

1. **Origin**: System calls are initiated by user programs when they request services from the kernel¹. On the other hand, interrupts are usually triggered by hardware components notifying the CPU/Microprocessor about an event that needs handling in software².

2. **Purpose**: System calls are used to request a service from the kernel¹. Interrupts, however, are used to alert the kernel to an event that has occurred¹.

3. **Mode of Operation**: System calls operate in user mode and then switch to kernel mode¹. Interrupts, however, operate directly in kernel mode¹.

4. **Response Time**: System calls have a predictable response time as they are serviced as soon as the kernel gets control¹. Interrupts, on the other hand, are serviced immediately, leading to an unpredictable response time¹.

5. **Control Transfer**: In a system call, control is transferred from the user program to the operating system kernel¹. In an interrupt, control is transferred from the currently executing process to the interrupt service routine¹.

Please note that these differences are not exclusive to Linux, but are generally applicable to most operating systems.
