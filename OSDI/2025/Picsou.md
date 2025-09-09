# Picsou: Enabling Replicated State Machines to Communicate Efficiently

## Abstract
Replicated state machines (RSMs) cannot communicate effec-
tively today as there is no formal framework or efficient pro-
tocol to do so. To address this issue, we introduce a new prim-
itive, Cross-Cluster Consistent Broadcast (C3B) and present
PICSOU, a practical implementation of the C3B primitive.
PICSOU draws inspiration from networking and TCP to allow
two RSMs to communicate with constant metadata overhead
in the failure-free case and a minimal number of message
resends in the case of failures. PICSOU is flexible and allows
both crash fault tolerant and Byzantine fault tolerant con-
sensus protocols to communicate. At the heart of PICSOU’s
good performance and generality is the concept of QUACKs
(quorum acknowledgments). QUACKs allow nodes in each
RSM to precisely determine when messages have definitely
been received, or likely lost. Our results are promising: we
obtain up to 24×better performance than prior solutions on
microbenchmarks and applications, ranging from disaster re-
covery to data reconciliation.

## People
Reginald Frank, Micah Murray, Chawinphat Tankuranand, Junseo Yoo, Ethan Xu, Natacha Crooks, Suyash Gupta†, Manos Kapritsos*
University of California, Berkeley; †University of Oregon;*University of Michigan