# Quantum Virtual Machines

## Abstract
Cloud computing services offer time on quantum computers,
but users are forced to each use the entire quantum computer
to run their programs as there is no way to multiplex a quan-
tum computer among multiple programs at the same time. We
present HyperQ, a system that introduces virtual machines for
quantum computers to provide fault isolation, better resource
utilization, and lower latency for quantum cloud computing.
A quantum virtual machine is defined in terms of quantum
computer hardware, specifically its quantum gates and qubits
arranged in a hardware-specific topology. HyperQ enables
quantum virtual machines to be simultaneously executed to-
gether on a quantum computer by multiplexing them in time
and space on the hardware and ensuring that they are iso-
lated from one another. HyperQ works with existing quantum
programs and compiler frameworks; programs are simply
compiled to run in virtual machines without the programs or
compilers needing to know what else might be executed at the
same time. We have implemented HyperQ for the IBM quan-
tum computing service, the largest quantum computing fleet
in the world. Our experimental results running quantum pro-
grams in virtual machines using the IBM service demonstrate
that HyperQ can increase utilization and throughput while
reducing program latency, by up to an order of magnitude,
without sacrificing, and in some cases improving, fidelity in
the results of quantum program execution.

## People
University of Maryland, College Park
Columbia University
University of Toronto