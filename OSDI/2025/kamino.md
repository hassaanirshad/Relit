# Kamino: Efficient VM Allocation at Scale with Latency-Driven Cache-Aware Scheduling

## Abstract
In virtual machine (VM) allocation systems, caching repeti-
tive and similar VM allocation requests and associated reso-
lution rules is crucial for reducing computational costs and
meeting strict latency requirements. While modern allocation
systems distribute requests among multiple allocator agents
and use caching to improve performance, current schedulers
often neglect the cache state and latency considerations when
assigning each new request to an agent. Due to the high
variance in costs of cache hits and misses and the associ-
ated processing overheads of updating the caches, simple
load-balancing and cache-aware mechanisms result in high
latencies. We introduce Kamino, a high-performance, latency-
driven and cache-aware request scheduling system aimed at
minimizing end-to-end latencies. Kamino employs a novel
scheduling algorithm grounded in theory which uses partial
indicators from the cache state to assign each new request
to the agent with the lowest estimated latency. Evaluation of
Kamino using a high-fidelity simulator on large-scale pro-
duction workloads shows a 42% reduction in average request
latencies. Our deployment of Kamino in the control plane of a
large public cloud confirms these improvements, with a 33%
decrease in cache miss rates and 17% reduction in memory
usage.

## People
Rutgers University
Microsoft Research
Microsoft Azure