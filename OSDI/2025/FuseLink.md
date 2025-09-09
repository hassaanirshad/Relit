# Enabling Efficient GPU Communication over Multiple NICs with FuseLink

## Abstract
Machine learning (ML) clusters stack multiple network inter-
face cards (NICs) within each server to improve inter-server
GPU communication bandwidth. However, existing systems
fall short in fully utilizing NICs because of static GPU-NIC
bindings. This leads to bottlenecks at hot-spot NICs when
handling imbalanced communication in ML tasks. For ex-
ample, large language model serving instances may have dif-
ferent communication demands across NICs; expert-parallel
training tasks have imbalanced all-to-all traffic; and the em-
bedding transmission volumes during recommendation model
training vary across GPUs. To fully utilize all NICs, we pro-
pose FuseLink to enable efficient GPU communication over
multiple NICs. FuseLink extends inter-server network by in-
tegrating high-speed intra-server connections, and leverages
GPUs to efficiently relay traffic to idle NICs. We implement
FuseLink and integrate it into NCCL, so that ML applications
can benefit from FuseLink seamlessly without code modifi-
cations. Compared to NCCL, we demonstrate that FuseLink
achieves up to 212GBps bandwidth between two inter-server
GPUs and accelerates ML tasks with dynamic traffic patterns.
Specifically, it reduces the latencies of first-token generation
in LLM model servings by 1.04-2.73→, improves the training
throughput of mixture-of-experts model by up to 1.3→, and
accelerates deep learning recommendation model training by
up to 1.2x.

## People

iSINGLab, Hong Kong University of Science and Technology
University of Science and Technology of China 
MetaX Integrated Circuits
Massachusetts Institute of Technology
Peking University
Meta