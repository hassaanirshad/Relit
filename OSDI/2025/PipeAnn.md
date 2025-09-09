# Achieving Low-Latency Graph-Based Vector Search via Aligning Best-First Search Algorithm with SSD

## Abstract
We propose PipeANN, an on-disk graph-based approximate
nearest neighbor search (ANNS) system, which significantly
bridges the latency gap with in-memory ones. We achieve this
by aligning the best-first search algorithm with SSD character-
istics, avoiding strict compute-I/O order across search steps.
Experiments show that PipeANN has 1.14×–2.02×search
latency compared to in-memory Vamana, and 35.0% of the
latency of on-disk DiskANN in billion-scale datasets, without
sacrificing search accuracy.

## People
Tsinghua University

