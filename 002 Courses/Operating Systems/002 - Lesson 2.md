Tags: #OperatingSystem #OperatingSysteStructure

## Topics

1. System Components
2. Operating Systems Services 
3. System Calls and System Programs

---
## System Components

**Process Management**: 
- A **process** is only ONE instant of a program in execution. 
- There are many processes can be running in the same program.

**Five major activities of an operating system in regard to process management are:

1. Creation and deletion of user and system processes
2. Suspension and resumption of processes.
3. A mechanism for process synchronization
4. A mechanism for process communication
5. A mechanism for deadlock handling

**Creation and Deletion of user and system processes**:
- *Creation*: When a new process is needed, whether by user request (like opening an application) or system operation (like background service), the *operating system* is responsible for creating this process.
- *Deletion* When a process terminates (either normally or due to an error), the operating system must clean up.

**Suspension and Resumption of Processes**
- *Suspension*: A process may need to be temporarily halted (suspended) for various reasons, such as waiting for I/O operations to complete or for higher-priority processes to execute.
- *Resumption*: When conditions allow, a suspended process must be resumed.

**A mechanism for Process Synchronization**
- Processes often need to *coordinate* their actions, especially when sharing resources or data. *Synchronization* mechanisms ensure that processes can work together without causing data inconsistency or conflicts.

**A mechanism for Process Communication**
- Processes often need to *communicate* with each other to share data or coordinate actions. 
- *IPC(Inter-Process Communication)*  mechanisms facilitate this communication.

**A mechanism for Deadlock Handling**
- *Deadlock*: a situation where two ore more processes are unable to proceed because each is waiting for the other release resources.
- *Handling Deadlocks*: involves identifying when a deadlock has occurred, designing the system to avoid deadlocks through careful resource allocation and process design, using algorithms to ensure that deadlock conditions are not met, like the *Banker's Algorithm*, and taking action to recover from a deadlock, which may include terminating or restating processes, or preempting resources from processes.

