# Low End-to-End Latency atop a Speculative Shared Log with Fix-Ante Ordering

## Abstract
Today’s shared logs incur expensive coordination to
globally order records across storage shards before they can
deliver records to applications. This makes them unsuitable
for many modern applications that must process ingested data
as early as possible and realize low end-to-end (e2e) laten-
cies. We propose SpecLog, a new shared log abstraction that
delivers records by speculating the global order, allowing the
application’s computation and shared-log coordination to be
overlapped, thus reducing e2e latency. To enable accurate
speculations, we introduce fix-ante ordering, a novel ordering
mechanism that predetermines the global order and makes the
shards adhere to the predetermined order. With fix-ante order-
ing, shards, except in rare cases, can accurately predict where
their records will sit in the total order before global coordi-
nation. We build Belfast, an implementation of the SpecLog
abstraction and fix-ante ordering. Our experiments show that
Belfast offers lower e2e latencies than current shared logs
while preserving their elasticity, flexibility, and scalability.

## People
University of Illinois Urbana-Champaign