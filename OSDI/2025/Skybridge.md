# Skybridge: Bounded Staleness for Distributed Caches

## Abstract
Meta Platforms Inc. is a social media company whose prod-
ucts require high availability and low latency. Meta’s services
run in multiple geographic locations around the world and
use asynchronous replication to keep the numerous cached
copies of the datastore in sync. This setup reduces consis-
tency in order to meet availability and latency requirements.
Eventual consistency due to asynchronous replication causes
issues for Meta’s services, ranging from minor annoyances to
product-breaking bugs. Therefore, we ask: can we put mean-
ingful bounds on how long it takes writes to be visible while
maintaining the scalability afforded by eventual consistency?
In this work we present Skybridge, an out-of-band replica-
tion stream for providing bounded staleness for distributed
caches. Skybridge takes advantage of the fact that Meta’s
systems already have a reliable delivery stream and instead
focuses on real-time delivery of updates. Skybridge is comple-
mentary to the main replication pipeline and avoids correlated
failures while being lightweight. We show that Skybridge
helps provide 2-second bounded staleness for 99.99998% of
writes, while the main replication pipeline only achieves this
99.993% of the time. Skybridge is able to achieve this while
only being 0.54% the size of cache deployments.

## People
Meta Platforms Inc.
OpenAI