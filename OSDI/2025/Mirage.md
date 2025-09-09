# Mirage: A Multi-Level Superoptimizer for Tensor Programs

## Abstract
We introduce Mirage, the first multi-level superoptimizer
for tensor programs. A key idea in Mirage is µGraphs, a
uniform representation of tensor programs at the kernel,
thread block, and thread levels of the GPU compute hier-
archy. µGraphs enable Mirage to discover novel optimiza-
tions that combine algebraic transformations, schedule trans-
formations, and generation of new custom kernels. To nav-
igate the large search space, Mirage introduces a pruning
technique based on abstraction that significantly reduces
the search space and provides a certain optimality guaran-
tee. To ensure that the optimized µGraph is equivalent to
the input program, Mirage introduces a probabilistic equiva-
lence verification procedure with strong theoretical guaran-
tees. Our evaluation shows that Mirage significantly outper-
forms existing approaches even for DNNs that are widely
used and heavily optimized. Mirage is publicly available at
https : //github.com/mirage-project/mirage.

## People

Carnegie Mellon University
Peking University
Pennsylvania State University
Purdue University
Weizmann Institute of Science
