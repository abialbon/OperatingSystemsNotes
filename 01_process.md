# Processes

### What is a process?

A process is an instance of a program in execution. It's an entity that can be executed on a processor.

A program comprises of:
- Program code
- Program data (the heap and the stack)
- Process Control Block

### What is a process control block?

- A data structure created by the OS to identify and keep track of processes
- Consists of
	1. Identifier
	2. State
	3. Priority
	4. Program counter
	5. Memory pointers
	6. Contextual data
	7. I/O status
	8. Accounting info
- Contextual data consists of the data present in the registers when the program is in execution.

### What are process states (5-state process model)

- Various processes are executed and blocked by the scheduler/dispatcher, hence it's important to keep track of the current state of the process. 
- The various states are:
	- New *(The process control block has been created, but the process is not yet in the pool of processes being excuted)*
	- Exit *(The process has quit or stopped)*
	- Running *(The process is currently being executed by a processor)*
	- Ready *(The process can be executed if a processor is available)*
	- Blocked *(The process is waiting for I/O or other event)*
	- Suspended Ready *(The process is suspended but is not waiting for any event)*
	- Suspended Blocked *(The processes is suspended and is blocked as it is waiting for I/O or other event)*


