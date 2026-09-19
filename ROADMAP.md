# Nimesh Builds roadmap

This roadmap records direction, not release dates. Status reflects work with visible evidence; an idea is not a shipped feature.

## Now · Design and validation

**ClusterReplica:** make it easier to create a selected replica of a Kubernetes software environment inside a vCluster for development and integration tests.

- Collect concrete workflows from platform teams and application developers.
- Validate one small end-to-end slice: provision, connect, install a supported tool, and clean up.
- Define the initial Kubernetes/vCluster version pair and required capabilities.
- Identify which configuration can be reproduced and which dependencies need explicit adapters or manual setup.

The project is being planned. No implementation or compatibility result has been published yet.

## Next · A usable first slice

Proposed milestone: one namespaced custom resource creates an isolated development environment, returns a working connection method, and tracks TTL cleanup. A reproducible demo and observed cleanup results are the evidence needed to call this complete.

## Later · Selected replication

Proposed additions, subject to feasibility:

1. Discover selected host components and show an inspectable installation plan.
2. Recreate supported operators and configuration with include/exclude selectors and overrides.
3. Support explicitly authorized secrets and workload identity mappings.
4. Validate representative workloads such as Spark and Trino.
5. Expand the tested Kubernetes, runtime, cloud, and distribution combinations.

EKS, AKS, GKE, OpenShift, and RKE2 are candidate validation environments, not a current support claim. Kubernetes API versions, available capabilities, and adapter behavior matter more than a distribution label alone.

## How to influence the roadmap

Start an [Ideas discussion](https://github.com/nimeshbuilds/.github/discussions/categories/ideas). Describe the workflow, the cost of the problem, existing tools you've tried, and a concrete outcome that would help. Sanitized examples and reproducible experiments are especially useful.

[ClusterReplica project brief](projects/cluster-replica.md) · [Contributing](CONTRIBUTING.md) · [Announcements](https://github.com/nimeshbuilds/.github/discussions/categories/announcements)
