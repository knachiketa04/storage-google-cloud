## Hyperdisk Pool
Hyperdisk Storage Pools are pre-purchased bundles of capacity, throughput, and IOPS for Compute Engine. You can create and manage disks within these pools, allocating resources to applications as needed. This centralized management simplifies capacity planning, reduces costs, and streamlines operations by consolidating hundreds of disks into a single pool.

## How it works?
Hyperdisk Storage Pools let you create a pool with the total capacity and performance your workloads need, then create disks within it to attach to VMs. These disks can be created with larger sizes or performance limits than initially needed, simplifying planning and allowing for future growth. If workloads grow, you can increase the pool's provisioned capacity and performance, letting individual disks use more resources up to their defined limits. This consolidates disk management and reduces costs. However, if an Advanced capacity pool reaches full utilization, writes to all disks fail until space is freed. Active monitoring and understanding workload behavior during out-of-space errors is crucial. In Advanced performance pools, auto-grow helps prevent performance issues by increasing available IOPS if contention is detected.


## Types of Pools
**Standard Capacity Storage Pools**
Standard capacity storage pools allow you to add disks until the total provisioned capacity of all disks reaches the pool's limit. Disks in these pools use capacity like regular disks.

**Advanced Capacity Storage Pools**
Advanced capacity storage pools offer thin-provisioning and data reduction, allowing you to provision more disk space than physically available. Disks in these pools consume capacity based on actual data written after reduction, enabling over-provisioning. The pool's used capacity is determined by written data, not provisioned disk space, and can exceed provisioned capacity by up to 500%.


## References
[Documentation-About Hyperdisk Storage Pools](https://cloud.google.com/compute/docs/disks/storage-pools)