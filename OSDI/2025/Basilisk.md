# Basilisk: Using Provenance Invariants to Automate Proofs of Undecidable Protocols

## Abstract
Distributed protocols are challenging to design correctly. One
promising approach to improve their reliability is to use for-
mal verification to prove that a protocol satisfies a desired
safety property. These proofs require finding an inductive
invariant that holds in the initial states of the system, im-
plies safety, and is inductive over state transitions. Devising
an inductive invariant is a difficult task that prior work has
either required the developer to find manually by a painful
search process, or automated by constraining the protocol to
a decidable but restrictive fragment of logic.
In this work, we aim to automatically find inductive invari-
ants without restricting the logic. We achieve this with two
key insights. First, many of the complex inter-host properties
that prior work required the developer to provide can instead
be expressed using Provenance Invariants, a class of invari-
ants that relate a local variable in a host to its provenance, i.e.,
the protocol step that caused it to take on its current value. By
tracing the provenance of one host variable back to another
host’s actions, we can derive an invariant relating the two
hosts’ states. Second, we develop an algorithm called atomic
sharding to derive Provenance Invariants automatically by
statically analyzing the protocol’s steps.
We implement these ideas in a tool called Basilisk and ap-
ply it to 16 distributed protocols, including complex ones like
Multi-Paxos. Basilisk automatically finds inductive invariants
and proves their inductiveness, with little or no developer as-
sistance. In all cases, these generated inductive invariants are
sufficient for us to prove safety without needing to identify
any new invariants.

## People

1. [Tony Nuda Zhang](https://tonyzhangnd.github.io/)
2. [Keshav Singh](https://linkedin.com/in/keshav-singh-388916218)
3. [Tej Chajed](https://www.chajed.io/)
4. [Manos Kapritsos](https://web.eecs.umich.edu/~manosk/)
5. [Bryan Parno](https://www.andrew.cmu.edu/user/bparno/)