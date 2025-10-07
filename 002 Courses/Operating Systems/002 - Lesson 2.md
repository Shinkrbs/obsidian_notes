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

![[Pasted image 20251007211249.png]]

**Main-Memory Management**: 
- *Main Memory*: a large array of words or bytes. Each word or byte has its own address. 
- *Main Memory*: a repository of quickly accessible data shared by the CPU and I/O devices.

**The major activities of an operating system in regard to memory-management**:

1.  Keep track of which part of memory are currently being used and by whom
2. Decide which processes are loaded into memory when memory space becomes available
3. Allocate and deallocate memory space as needed.

**Keep track of which part of memory are currently being used and by whom**

- *OS* maintains a record of which parts of the memory are currently in use and which are free. 
- It uses data structures to track which memory addresses are allocated to processes and which are available. 
- This tracking ensures that *processes don't overlap or interfere with each other's memory*, which could leap to error or system crashes.

**Decide which processes are loaded into memory space becomes available**  
- When there's free memory space available, the OS *decides which processes to load into that space*. 
- The *OS schedules and manages to processes based on various criteria such as priority, memory requirements, and current system load*.
- The OS decides which processes to *load or swap in from disk storage when memory becomes available*
- This helps in efficiently utilizing memory and ensuring the active processes have the resources they need.

**Allocate and Deallocate memory space as needed.**
- The *OS handles the assignment of memory to processes* and then *reclaims that memory when it's no longer needed*.
- When a process requests memory, the *OS allocates a suitable block of memory from the free pool*
- When the process terminates or no loner needs certain memory, the *OS deallocates memory, making it available for other processes*. 
- This dynamic management ensures that memory is used efficiently and prevents fragmentation or wastage.

**File Management**
- A *file* is collected of related information defined by its creator.
- *Computer* can store files on the disk(secondary storage), which provide long term storage.

1. The creation and deletion files
2. The creation and deletion of directions
3. The support of primitives for manipulating files and directions
4. The mapping of files onto secondary storage
5. The backup of files on stable storage media

**The creation and deletion of files**
- *OS handles the process of creating new files and removing existing ones*
- When a file is created, the OS *allocates space on the disk and updates its directory* 
- *Deletion*:  removes the file's data and frees up space.

**The creation and deletion of directions**
- *OS manages the creation of directories(folders) and their removal. 
- *Directories*: help organize files
- The *OS updates the file system structure to reflect new directories or remove them as needed.*

**The support of primitives for manipulating files and directions**
- *OS provides basic operations (primitives) for interacting with files and directories.* 
- These operations include opening, reading, writing, closing files, and navigating directories. 
- They allow applications and users to manage file data and directory structures.

**The mapping of files onto secondary storage**
- *OS translates file data into specific locations on disk storage*
- It maintains a file allocation table or similar structure to keep track of where each file's data is stored on the disk.

**The backup of files on stable storage media**
- *OS ensures that files are backed up to prevent data loss*
- It involves copying files to backup storage media to safeguard against hardware failures or data corruption.

**I/O System Management**
- A purpose of an OS is to *hide the peculiarities of specific hardware devices from the user*. 
- The OS *provides a consistent and standardized interface for input and output operations, regardless of the specific hardware being used.*

**Secondary-Storage Management
- Levels of Storage: Primary Storage, Secondary Storage, and Cache Storage
- Instructions and data must be placed in *primary storage or cached storage* to be referenced by a running program

**Functions**
- *Main Memory*: When you run a program, the instructions and data needed by the CPU are loaded from secondary storage into primary storage. This allows the CPU to access this information quickly.
- *Secondary Storage*: used to store data and programs permanently. When a program is launched or data is needed, it is transferred from secondary storage to primary storage.
- *Cache Storage*: holds copies of data from the most frequently used main memory locations. When the CPU needs to access data, it firsts checks the cache. If the data is there (*cache hit*), it can be accessed much faster than if it had to be fetched from RAM. If the data is not found (*cache miss*), it is fetched from the RAM, and the cache is updated.

*Networking*: a distributed system is a collection of processors that do not share memory, peripheral devices, or a clock. The processors communicate with one another through communication lines called *network*.

*Protection System*: 
- *Protection*: mechanism for controlling the access of programs, processes, or users to the resources defined by a computer system. 
- *Primary Purpose of Protection System*: to ensure the integrity, confidentiality, and availability of resources within a computer system. This helps prevents unauthorized access, data breaches, and potential damage to the system's operation.

---
## Operating System Services

*Program Execution*: The system must be able to load a program into memory and to run it. The program must be able to end its execution, either normally or abnormally (indicating error).

*I/O Operations*: A running program may require I/O. This I/O may involve file or an I/O device.

*File System Manipulation*: The output of a program may need to be written into new files or input taken from some files. The operating system provides this service.

*Error Detection*: An error is one part of the system may cause malfunctioning of the complete system. To avoid such a situation the operating system constantly monitors the system from detecting the errors.

---
## System Calls and System Programs

**System Calls**:
- provide the interface between a process and the operating system.
- these calls are generally available as assembly-language instructions, and are usually listed in the manuals used by assembly language programmers.
- mostly accessed by programs via a high-level API rather than direct system call use.

**Purpose**: since user-level processed do not have direct access to the underlying hardware or critical system resources, they rely on system calls to perform tasks that require privileged access.

![[Pasted image 20251008032454.png]]
![[Pasted image 20251008032505.png]]
![[Pasted image 20251008032523.png]]

**System Programs**:
- provides a layer between the user and the operating system. 
- these programs support and manage the operation of the OS and help users and system administrators perform various tasks related to system management, resource allocation, and program execution.
- File manipulation, Status Information, File modification, Programming language support, Program loading and execution, Communications, Applications programs.
- Most users view of the OS is *defined by system programs*, not the actual system calls.