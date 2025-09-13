# QiMeng-Xpiler: Transcompiling Tensor Programs for Deep Learning Systems with a Neural-Symbolic Approach

## Abstract
Heterogeneous deep learning systems (DLS) such as GPUs
and ASICs have been widely deployed in industrial data cen-
ters, which requires to develop multiple low-level tensor pro-
grams for different platforms. An attractive solution to relieve
the programming burden is to transcompile the legacy code
of one platform to others. However, current transcompilation
techniques struggle with either tremendous manual efforts or
functional incorrectness, rendering “Write Once, Run Any-
where” of tensor programs an open question.
We propose a novel transcompiler, i.e., QiMeng-Xpiler, for
automatically translating tensor programs across DLS via
both large language models (LLMs) and symbolic program
synthesis, i.e., neural-symbolic synthesis. The key insight is
leveraging the powerful code generation ability of LLM to
make costly search-based symbolic synthesis computation-
ally tractable. Concretely, we propose multiple LLM-assisted
compilation passes via pre-defined meta-prompts for program
transformation. During each program transformation, effi-
cient symbolic program synthesis is employed to repair in-
correct code snippets with a limited scale. To attain high
performance, we propose a hierarchical auto-tuning approach
to systematically explore both the parameters and sequences
of transformation passes. Experiments on 4 DLS with dis-
tinct programming interfaces, i.e., Intel DL Boost with VNNI,
NVIDIA GPU with CUDA, AMD MI with HIP, and Cam-
bricon MLU with BANG, demonstrate that QiMeng-Xpiler
correctly translates different tensor programs at the accuracy
of 95% on average.

## People
