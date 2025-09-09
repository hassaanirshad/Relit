# Quake: Adaptive Indexing for Vector Search

## Abstract
Vector search, the task of finding the k-nearest neighbors
of a query vector against a database of high-dimensional vec-
tors, underpins many machine learning applications, includ-
ing retrieval-augmented generation, recommendation systems,
and information retrieval. However, existing approximate
nearest neighbor (ANN) methods perform poorly under dy-
namic and skewed workloads where data distributions evolve.
We introduce Quake, an adaptive indexing system that main-
tains low latency and high recall in such environments. Quake
employs a multi-level partitioning scheme that adjusts to up-
dates and changing access patterns, guided by a cost model
that predicts query latency based on partition sizes and access
frequencies. Quake also dynamically sets query execution
parameters to meet recall targets using a novel recall estima-
tion model. Furthermore, Quake utilizes NUMA-aware intra-
query parallelism for improved memory bandwidth utilization
during search. To evaluate Quake, we prepare a Wikipedia
vector search workload and develop a workload generator
to create vector search workloads with configurable access
patterns. Our evaluation shows that on dynamic workloads,
Quake achieves query latency reductions of 1.5–38×and up-
date latency reductions of 4.5–126×compared to state-of-the-
art indexes such as SVS, DiskANN, HNSW, and SCANN.

## People
University of Wisconsin-Madison
Apple
University of Waterloo