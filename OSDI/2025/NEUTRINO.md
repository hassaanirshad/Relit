# NEUTRINO: Fine-grained GPU Kernel Profiling via Programmable Probing

## Abstract
As GPUs play an increasingly important role in computer
systems in the scaling laws era, understanding fine-grained
GPU runtime behavior is more crucial than ever. However,
existing GPU kernel profilers, typically kernel-exclusive or
hardware-dependent, often fail to capture fine-grained mea-
surements. This paper presents NEUTRINO, a programmable
interface for GPU kernel profiling that leverages assembly-
layer probing to achieve instruction-level fine granularity, pro-
filing versatility across time and value domains, and hardware
independence. To better visualize the rich details captured
by NEUTRINO, we introduce the Densified Memory Access
Timeline (DMAT), a novel representation that offers new in-
sights into GPU runtime behavior. We implement NEUTRINO
in Linux for both NVIDIA and AMD GPUs and conduct
extensive evaluations and analyses. The results demonstrate
NEUTRINO’s superior capabilities in GPU kernel profiling
with low overhead. We envision NEUTRINO as a valuable
tool for the community and have open-sourced it to facilitate
future research at https://github.com/open-neutrino/
neutrino.

## People
Songlin Huang & Chenshu Wu @ The University of Hong Kong