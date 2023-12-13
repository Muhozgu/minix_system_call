**Step 1: Understand the Existing Code**

Make sure you understand the existing codebase, especially the structure of system calls, and how they are implemented in Minix. Review the class recording for the presentation on implementing system calls, especially the getchildren system call.

**Step 2: Implement getchildren System Call**

Follow the example from the class recording to implement the getchildren system call. This might involve updating the system call table, defining the system call function, and handling the request in the kernel.

**Step 3: Implement do_get_parent_pid System Call**

Create a new system call named do_get_parent_pid. Define the constant PM_GETPARENTPID to identify this new system call. Update the system call table to include the new entry for do_get_parent_pid.

**Step 4: Write Implementation for do_get_parent_pid**

Implement the do_get_parent_pid function in the kernel. This function should return the parent PID of the process that executed the system call. You might need to traverse the process data structures to find the parent process.

**Step 5: Update User-Space Program**

Write a user-space program that demonstrates the usage of the new system call. The program should have two processes: a parent and a child. The parent process should display its PID, and the child process should use the do_get_parent_pid system call and display the returned value.
