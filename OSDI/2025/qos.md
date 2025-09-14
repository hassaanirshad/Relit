# QOS: Quantum Operating System

## Abstract
Quantum computers face challenges due to hardware
constraints, noise errors, and heterogeneity, and face
fundamental design tradeoffs between key performance
metrics such as quantum fidelity and system utilization. This
substantially complicates managing quantum resources to
scale the size and number of quantum algorithms that can
be executed reliably in a given time.
We introduce QOS, a modular quantum operating system
that holistically addresses the challenges of quantum resource
management by systematically exploring key design tradeoffs
across the stack. QOS exposes a hardware-agnostic API for
transparent quantum job execution, mitigates hardware
errors, and systematically multi-programs and schedules
the jobs across space and time to achieve high quantum
fidelity in a resource-efficient manner. QOS’s modular design
enables synergistic cross- and intra-layer optimizations,
while introducing new concepts such as compatibility-based
multi-programming and effective utilization.
We evaluate QOS on real quantum devices hosted by IBM,
using 7000 real quantum runs of more than 70.000 benchmark
instances. We show that the QOS achieves 2.6–456.5×higher
fidelity, increases resource utilization by up to 9.6×, and
reduces waiting times by up to 5×while sacrificing only
1–3% fidelity, on average, compared to the baselines.

## People
Technical University of Munich