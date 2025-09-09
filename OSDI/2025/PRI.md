# To PRI or Not To PRI, That’s the question

## Abstract
SR-IOV and I/O device passthrough enable network and
storage devices to be shared among multiple tenants with
high density using virtual functions (VFs), achieving near-
native performance. However, passthrough does not support
page faults, requiring the hypervisor to statically pin the VM-
allocated memory. This approach is unacceptable for cloud
service providers (CSPs) that rely on oversubscription to en-
hance memory utilization and reduce costs. The Page Request
Interface (PRI) was designed to support device-side I/O page
faults (IOPFs) through collaboration among devices, Input-
Output Memory Management Units (IOMMU), and the OS.
But PRI has not seen broad adoption in devices like NICs and
storage.
We propose VIO, a novel dynamic I/O device passthrough
approach that achieves near-native performance and is
hardware-independent. By leveraging a shadow available
queue, VIO can dynamically and transparently switch devices
between VIO and passthrough modes based on I/O operations
per second (IOPS) pressure, balancing resource utilization
and performance. Each DMA request is probed via IOPA-
snooping in the virtio data plane to eliminate IOPFs, while
device interrupts are directly passed through to the VM guest,
enabling performance close to passthrough. VIO is exten-
sively tested and deployed by a leading global CSP across
300K VMs, supporting both legacy and new instances while
reclaiming up to the equivalent of 30K VM memory daily
without compromising user Service Level Objectives (SLOs).
As the scale grows, the benefits continue to increase.

## People

Shanghai Jiao Tong University & Alibaba Group