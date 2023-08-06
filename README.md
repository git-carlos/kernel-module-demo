# Kernel Module Demonstration
Constructed by Carlos Pantoja-Malaga & Stanley Vossler

Revisions done by Carlos Pantoja-Malaga for GitHub Repository ```kernel-module-demo```.

## Description
Through the compilation and execution of the module files the program simulates a barstool scheduler through kernel signal calling.

sys_call.c is a C file which defclares system calls intialize_bar(), customer_arrival(), close_bar(). barstool.c is a file which defines the system call behavior. barstool.c acts as a bar scheduler in which a waiter operates on a seperate kernel thread interacting with bar data available.

In order to compile `kernel-module-demo`, clone the GitHub Repository and execute `make`.

Make sure that system calls intialize_bar, customer_arrival, and close_bar are defined in `(KERNELDIR)/arch/x86/entry/syscall/syscall_64.tbl` as labels 548, 549, and 550 - respectively. Make sure the system calls are also defined in `(KERNELDIR)/include/linux/syscalls.h`. Finally in the `/lib/modules/5.15.102/build/Makefile` make sure the directory where all the source files is defined like so, `core-y+=kernel/certs/mm/fs/ipc/security/crypto/(DIRECTORYNAME)/`.

## Project Milestones
|Milestone|Description|
|---|---|
|||
|||
|||

## Revision Documentation

## Epilogue
