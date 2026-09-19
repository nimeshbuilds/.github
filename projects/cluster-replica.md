# ClusterReplica

**An experimental Kubernetes operator for reproducible development environments built on vCluster.**

Status: **early runtime prototype**. [Explore the code and quickstart](https://github.com/nimeshbuilds/cluster-replica). The initial operator provisions a pinned vCluster and manages limited Helm-release TTL cleanup. Automatic host replication, complete cleanup, production releases, and compatibility certification are still ahead.

## The problem

An empty test cluster often misses the operators and configuration that applications depend on. Rebuilding the environment by hand is slow, and a shared development namespace can make experiments interfere with each other.

## The proposed workflow

An administrator installs the wrapper operator and grants a bounded set of discovery, provisioning, and access permissions. A developer applies one `ClusterReplica` resource to request a vCluster and a selected set of source components.

The operator would:

1. Detect the host's Kubernetes version, APIs, and required capabilities.
2. Use an authorized existing vCluster integration or provision a new vCluster.
3. Discover the selected operators and configuration, resolve dependencies, and produce an inspectable plan.
4. Recreate supported components with namespace, Helm value, storage, domain, and identity overrides.
5. Return scoped access for people, CI, or agents, with status showing what was verified.
6. Track owned resources and clean them up on deletion or TTL expiry.

## Boundaries to validate

- A virtual cluster shares host infrastructure. It does not clone cloud control planes, worker nodes, accounts, or external services.
- Secrets require explicit permission and selection. A development environment must not silently receive all production credentials.
- Workload identity requires the correct target identity and cloud trust configuration; copying a service-account annotation alone is insufficient.
- Storage and external data need explicit isolation or sharing rules. TTL is a cleanup trigger, not proof that every external resource or retained snapshot has disappeared.
- Spark, Trino, and other heavy workloads still depend on the host's capacity, isolation, storage, and networking.
- Compatibility must be demonstrated for the selected Kubernetes/vCluster versions and adapters. No universal distribution support is claimed.

## First useful evidence

A small, repeatable demo should show a request becoming a usable vCluster, a supported component working inside it, and its owned resources being removed at expiry. That evidence should precede expanding the support matrix.

This project intends to build on [vCluster](https://www.vcluster.com/), not replace it. Nimesh Builds is an independent project and is not affiliated with or endorsed by the vCluster maintainers.

[Discuss the use case](https://github.com/nimeshbuilds/.github/discussions/categories/ideas) · [Roadmap](../ROADMAP.md) · [Contribute](../CONTRIBUTING.md)
