# Mako: Speculative Distributed Transactions with Geo-Replication

## Abstract
This paper introduces Mako, a highly available, high-
throughput, and horizontally scalable transactional key-value
store. Mako performs strongly consistent geo-replication to
maintain availability despite entire datacenter failures, uses
multi-core machines for fast serializable transaction process-
ing, and shards data to scale out. To achieve these properties,
especially to overcome the overheads of distributed transac-
tions in geo-replicated settings, Mako decouples transaction
execution and replication. This enables Mako to run transac-
tions speculatively and very fast, and replicate transactions
in the background to make them fault-tolerant. The key inno-
vation in Mako is the use of two-phase commit (2PC) specu-
latively to allow distributed transactions to proceed without
having to wait for their decisions to be replicated, while also
preventing unbounded cascading aborts if shards fail prior to
the end of replication. Our experimental evaluation on Azure
shows that Mako processes 3.66M TPC-C transactions per
second when data is split across 10 shards, each of which
runs with 24 threads. This is an 8.6×higher throughput than
state-of-the-art systems optimized for geo-replication.

## People
Stony Brook University
Google
Microsoft Research
University of Pennsylvania