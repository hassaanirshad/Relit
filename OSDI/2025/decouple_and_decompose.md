# Decouple and Decompose: Scaling Resource Allocation with DEDE

## Abstract
Efficient resource allocation is essential in cloud systems
to facilitate resource sharing among tenants. However, the
growing scale of these optimization problems have outpaced
commercial solvers commonly employed in production. To ac-
celerate resource allocation, prior approaches either customize
solutions for narrow domains or impose workload-specific
assumptions. In this work, we revisit real-world resource allo-
cation problems and uncover a common underlying structure:
the vast majority of these problems are inherently separable,
i.e., they optimize the aggregate utility of individual resource
and demand allocations, under separate constraints for each
resource and each demand. Building on this observation, we
develop DEDE, a scalable and theoretically rooted optimiza-
tion framework for large-scale resource allocation. At the
core of DEDE is a decouple-and-decompose approach: it
decouples entangled resource and demand constraints and
thereby decomposes the overall optimization into alternat-
ing per-resource and per-demand subproblems that can be
solved efficiently and in parallel. We have implemented and
released DEDE as a Python package with a familiar modeling
interface. Our experiments on three representative resource
allocation tasks—cluster scheduling, traffic engineering, and
load balancing—demonstrate that DEDE delivers significant
speedups while generating higher-quality allocations.

## People
Harvard University 
University of Illinois Urbana-Champaign