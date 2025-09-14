# Principles and Methodologies for Serial Performance Optimization

## Abstract
Throughout the history of computer science, optimizing
existing systems to achieve higher performance has been a
longstanding aspiration. While the primary emphasis of this
endeavor lies in reducing latency and increasing throughput,
these two are closely intertwined, and answering the how
question has remained a challenge, often relying on intuition
and experience.
This paper introduces a systematic approach to optimizing
sequential tasks, which are fundamental for overall perfor-
mance. We define three principles—task removal, replace-
ment, and reordering—and distill them into eight actionable
methodologies: batching, caching, precomputing, deferring,
relaxation, contextualization, hardware specialization, and
layering. Our review of OSDI and SOSP papers over the past
decade shows that these techniques, when taken together,
comprehensively account for the observed sequential opti-
mization strategies.
To illustrate the framework’s practical value, we present
two case studies: one on file and storage systems, and another
analyzing kernel synchronization to uncover missed opti-
mization opportunities. Furthermore, we introduce SysGPT,
a fine-tuned GPT model trained on curated literature anal-
ysis, which offer context-aware performance suggestions.
SysGPT’s outputs are more specific and feasible than GPT-4’s,
aligning with core strategies from recent research without
direct exposure, demonstrating its utility as an optimization
assistant.

## People
Georgia Institute of Technology