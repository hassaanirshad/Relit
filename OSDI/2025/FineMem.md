# FineMem: Breaking the Allocation Overhead vs. Memory Waste Dilemma in Fine-Grained Disaggregated Memory Management

## Abstract
RDMA-enabled memory disaggregation has emerged as
an attractive approach to reducing memory costs in mod-
ern data centers. While RDMA enables efficient remote
read/write operations,it presents challenges in remote mem-
ory (de)allocation. Consequently, existing systems adopt
coarse-grained allocations (inGBs), leading to memory waste.
We introduce FineMem, an RDMA-connected remote
memory management system that enables high-performance,
fine-grained memoryallocation. FineMem addresses latency
and scalability challenges related to fine-grained allocations.
It removes RDMA memory region (MR) registration costs
from allocation paths through per-compute node MR pre-
registration, while ensuring remote memory isolation using
RDMA memory windows and a trusted allocation service
on each compute node. It employs a lock-free, one-sided
RDMA-based protocol to allocate memory chunks (e.g.,4KB,
2MB) without involving the memory node’s CPU and main-
tains metadata consistency during compute node failures via
logging. We show that FineMem reduces remote memory
allocation latency by as much as 95% compared to state-
of-the-art remote memory management systems. It enables
memory malloc systems, key-value stores systems, and swap
systems running on FineMem to achieve low memory waste
with minimal overhead.

## People

1. Xiaoyang Wang & Yongkun Li & Wenzhe Zhu & Yuqi Li @ University of Science and Technology of China
2. Kan Wu @ Google
3. Yinlong Xu @ Anhui Provincial Key Laboratory of High Performance Computing, USTC