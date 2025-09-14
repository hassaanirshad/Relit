# Understanding Stragglers in Large Model Training Using What-if Analysis

## Abstract
Large language model (LLM) training is one of the most
demanding distributed computations today, often requiring
thousands of GPUs with frequent synchronization across ma-
chines. Such a workload pattern makes it susceptible to strag-
glers, where the training can be stalled by few slow work-
ers. At ByteDance we find stragglers are not trivially always
caused by hardware failures, but can arise from multiple com-
plex factors. This work aims to present a comprehensive study
on the straggler issues in LLM training, using a five-month
trace collected from our ByteDance LLM training cluster.
The core methodology is what-if analysis that simulates the
scenario without any stragglers and contrasts with the actual
case. We use this method to study the following questions: (1)
how often do stragglers affect training jobs, and what effect
do they have on job performance; (2) do stragglers exhibit
temporal or spatial patterns; and (3) what are the potential
root causes for stragglers?

## People
New York University
ByteDance Seed
ByteDance
Zhejiang University