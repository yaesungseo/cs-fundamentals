# Computer Hardware
## Core idea
A computer combines computation, memory, storage, and input/output. Performance depends on the workload and on how data moves between these components.

## CPU, GPU, and FPGA
- **CPU — Central Processing Unit:** a general-purpose processor suited to varied instruction sequences and control flow. Modern CPUs have multiple cores and also support parallel execution.
- **GPU — Graphics Processing Unit:** a processor designed for high throughput across many parallel operations. Graphics and large numerical workloads can benefit when enough independent work is available.
- **FPGA — Field-Programmable Gate Array:** reconfigurable hardware whose logic and interconnections can be configured to implement a circuit. Hardware description languages describe circuits; FPGA development is not simply running ordinary CPU instructions faster.

A GPU is not automatically faster than a CPU. Data transfer, branching, problem size, and memory access patterns matter. An FPGA is not a universal replacement for either processor.

## Memory hierarchy
Registers and caches keep frequently needed data close to execution units. RAM holds active program data; SSDs and hard drives provide persistent storage. Typical main memory loses its contents when power is removed.

**Latency** measures how long an operation takes. **Throughput** measures how much work completes per unit of time. Improving one does not necessarily improve the other.

## Example
A large image transformation may apply the same calculation to millions of pixels, making parallel execution useful. A small, branch-heavy task may not justify transferring data to a GPU.

## Try it
Explain why adding storage capacity does not necessarily make a program with insufficient RAM run efficiently.

## Expand next
Bits and bytes; binary and hexadecimal; logic gates; instruction sets; cache locality; buses; accelerators.

[Back to index](../../README.md)
