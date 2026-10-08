# Operating Systems
## Core idea
An operating system manages hardware resources and provides services that programs use through interfaces such as system calls.

## Essential vocabulary
- **Program:** instructions and associated data.
- **Process:** an executing program instance with resources such as an address space.
- **Thread:** an execution sequence within a process; threads typically share the process's memory.
- **Scheduler:** chooses which runnable threads or processes get processor time.
- **Virtual memory:** gives processes virtual address spaces mapped to underlying memory resources. It is broader than swapping data to disk.

## Concurrency and parallelism
Concurrency means tasks can make progress during overlapping periods. Parallelism means tasks execute at the same time. A single CPU core can interleave concurrent tasks without executing them simultaneously.

Shared memory introduces coordination problems. Two threads incrementing the same counter can lose updates if the read-modify-write sequence is not appropriately synchronized. Locks can protect shared state, but inconsistent lock ordering can cause deadlock.

## Example
A browser can remain responsive while waiting for network data because waiting and computation can be coordinated without blocking all work.

## Common confusion
The call stack and dynamically allocated memory are memory-management concepts. A heap data structure is a different concept; see the companion algorithms repository.

## Try it
Write down a possible interleaving of two unsynchronized increments that produces only one net increment.

## Expand next
System calls; context switches; stack and dynamic allocation; paging; filesystems; race conditions; deadlock conditions.

[Back to index](../../README.md)
