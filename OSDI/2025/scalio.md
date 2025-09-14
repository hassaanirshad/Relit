# Scalio: Scaling up DPU-based JBOF Key-value Store with NVMe-oF Target Offload

## Abstract
The rapid growth of data-intensive applications has created a
demand for high-density storage systems. Data-Processing-
Unit-based (DPU-based) Just a Bunch of Flash (JBOF) so-
lutions provide an energy-efficient and cost-effective archi-
tecture to meet this need. However, existing JBOF solutions
struggle with scalability when handling an increasing number
of attached SSDs, due to their heavy reliance on the DPU’s
CPU for SSD I/O operations.
In this paper, we introduce Scalio, a scalable disaggregated
key-value store designed to address the limitations of current
DPU-based JBOF systems. Scalio offloads as many SSD I/O
operations as possible to the DPU’s network I/O capabili-
ties, including traditional RDMA verbs and a recent hardware
optimization, NVMe over Fabrics Target Offload. Addition-
ally, Scalio incorporates a two-layer design with compact
in-memory data structures to handle hot read traffic and man-
age bursty writes. One of the key challenges in this design is
ensuring consistency between the DRAM states in the DPU
and the SSD states, which, unlike CPU L1/L2 caches, are not
automatically synchronized through hardware cache coher-
ence protocols. To address this, Scalio introduces an RDMA-
based cache consistency protocol that guarantees linearizabil-
ity across the system, despite the disaggregated nature of the
architecture.
Our experiments show that Scalio significantly improves
both scalability and throughput, achieving up to 3.3× higher
throughput compared to existing systems, especially in high-
density SSD configurations.

## People
Tsinghua University
Quan Cheng Laboratory