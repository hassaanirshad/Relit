# Tigon: A Distributed Database for a CXL Pod

## Abstract
Building efficient distributed transactional databases remains
a challenging problem despite decades of research. Existing
distributed databases synchronize cross-host concurrent data
accesses over a network, which requires numerous message
exchanges and introduces performance overhead.
We describe Tigon, the first distributed in-memory database
that synchronizes concurrent cross-host data accesses using
atomic operations on CXL memory. Using CXL memory is
more efficient than network-based approaches, but Tigon’s de-
sign must address CXL’s higher latency and lower bandwidth
relative to local DRAM, as well as CXL’s limited hardware sup-
port for cross-host cache coherence. For TPC-C and a variant
of YCSB, Tigon achieves up to 2.5×higher throughput com-
pared with two optimized shared-nothing databases that use
CXL memory as a transport and up to 18.5×higher throughput
compared with an RDMA-based distributed database.

## People
The University of Texas at Austin 
University of Illinois Urbana-Champaign