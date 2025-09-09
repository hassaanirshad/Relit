# KPerfIR: Towards an Open and Compiler-centric Ecosystem for GPU Kernel Performance Tooling on Modern AI Workloads

## Abstract
In this work, we propose KPerfIR, a novel multilevel
compiler-centric infrastructure to enable the development of
customizable, extendable, and portable profiling tools tailored
for modern artificial intelligence (AI) workloads on modern
GPUs. Our approach integrates profiling capabilities directly
into the compiler workflow, allowing profiling functionali-
ties to be implemented as compiler passes, offering a pro-
grammable and reusable framework for performance analysis.
This design bridges the gap between compilers and profil-
ers, enabling fine-grained insights into complex optimization
challenges such as overlapping the execution of fine-grained
function units on GPUs. KPerfIR is integrated into the Triton
infrastructure to highlight the power of a compiler-centric ap-
proach to advance performance analysis and optimization in
the ever-evolving landscape of AI compilers. Our evaluation
shows that our tool incurs low overhead (8.2%), provides accu-
rate measurements (2% relative error), and delivers actionable
insights into complicated GPU intra-kernel optimizations.

## People
Yufei Ding & Zhongkai Yu & Yue Guan @ University of California, San Diego
Yuanwei Fang & Adnan Aziz & Corbin Robeck & Manman Ren @ Meta
Keren Zhou @ George Mason University
OpenAI