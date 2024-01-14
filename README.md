# Linux-kernel-questions
A few question about Linux kernel and tracing tools

**What is interrupts and system calls in OS?**
answer:
Sure, let's discuss these two important concepts in operating systems:

1. **System Call**: A system call is a method that enables a user process to interact with the kernel of the operating system¹. It's a call from user mode to kernel mode¹. We can use system calls to read information from files, get time, manage the computer’s memory, or control the data flow between computers¹. A user program initiates a system call by executing an instruction that transfers control from the user program to the operating system kernel¹. System calls can be divided into five categories based on their use: process control, maintenance of information, management of participating devices, handling communication, and file management¹.

2. **System Interrupt**: System interrupts are a way for a process to alert the kernel that an event has occurred¹. Once interrupted, the kernel can process the event and return to the process where it left off¹. An interrupt is an alert triggered by events such as the completion of an instruction, hardware or software signaling for an event, and timers reaching their final countdown value¹. Interrupts can be initiated from software to implement concurrency control mechanisms¹. They can also arise in response to some asynchronous event¹. Interrupts can be divided into two types: software interrupts and hardware interrupts². Software interrupts are produced by software or a system, often to carry out a certain function or respond to an error condition². Hardware interrupts are signals emitted by hardware when a process or an event needs immediate attention².

In summary, both system calls and system interrupts are ways for user processes to communicate with the OS kernel directly¹. However, a system call is a request by a program to the kernel for the execution of an operation, while an interrupt is an alert triggered by events requiring immediate attention¹..

