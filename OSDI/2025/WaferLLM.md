# WaferLLM: Large Language Model Inference at Wafer Scale

## Abstract
Emerging AI accelerators increasingly adopt wafer-scale
manufacturing technologies, integrating hundreds of thou-
sands of AI cores in a mesh architecture with large distributed
on-chip memory (tens of GB in total) and ultra-high on-chip
memory bandwidth (tens of PB/s). However, current LLM
inference systems, optimized for shared memory architectures
like GPUs, fail to exploit these accelerators fully.
We introduce WaferLLM, the first wafer-scale LLM infer-
ence system. WaferLLM is guided by a novel PLMR model
(pronounced as "Plummer") that captures the unique hardware
characteristics of wafer-scale architectures. Leveraging this
model, WaferLLM pioneers wafer-scale LLM parallelism, op-
timizing the utilization of hundreds of thousands of on-chip
cores. It also introduces MeshGEMM and MeshGEMV, the
first GEMM and GEMV implementations designed to scale
effectively on wafer-scale accelerators.
Evaluations show that WaferLLM achieves up to 200×
higher accelerator utilization than state-of-the-art methods.
Leveraging a wafer-scale accelerator (Cerebras WSE2),
WaferLLM delivers GEMV operations 606×faster and 16×
more energy-efficient than on an NVIDIA A100 GPU. For
full LLM inference, WaferLLM achieves 10-20×speedups
over A100 GPU clusters running SGLang and vLLM. These
advantages are expected to grow as wafer-scale AI models,
software, and hardware continue to mature. WaferLLM is
open-sourced at https://github.com/MeshInfra/WaferLLM.

## People
University of Edinburgh
Microsoft Research