# Fork in the Road: Reflections and Optimizations for Cold Start Latency in Production Serverless Systems

## Abstract
Serverless computing has seen widespread adoption in pub-
lic cloud environments. However, it continues to suffer from
long cold start latency, which remains a key performance
bottleneck. We have conducted an in-depth investigation of
existing cold start optimizations and evaluated their effective-
ness in large-scale industrial deployments. Our study reveals
several common limitations in prior research: (1) reliance
on simplified assumptions that overlook the complexities of
large-scale systems; (2) a narrow focus on optimizing isolated
components of the cold start process, while ignoring end-to-
end workflow interactions; and (3) insufficient attention to the
challenges introduced by concurrent execution environments.
As a result, despite incorporating prior techniques, cold start
latency on the Ant Group serverless platform remains in the
range of hundreds of milliseconds to several seconds.
This paper identifies three previously overlooked sources of
latency: (1) control path latency, stemming from interactions
within the serverless runtime; (2) resource contention latency,
arising under high concurrency and sustained execution; and
(3) user code initialization latency, which reflects the trade-off
between resource efficiency and startup performance. To ad-
dress these challenges, we propose a suite of novel techniques
that overcome key limitations in existing approaches. These
techniques are designed to be both adaptable to real-world
workloads and scalable to large deployments. Our system,
AFaaS (short for Ant FaaS), reduces cold start latency to the
millisecond level. AFaaS has been deployed in production
for over 18 months and has consistently demonstrated stable
performance at scale.

## People
Tsinghua University
Ant Group
Shanghai Jiao Tong University
Quan Cheng Laboratory