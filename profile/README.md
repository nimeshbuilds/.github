<p align="center">
  <img src="https://raw.githubusercontent.com/nimeshbuilds/.github/main/assets/banner.png" alt="Nimesh Builds — Vibe coding. Open source. Built in public." width="100%">
</p>

# Open-source Kubernetes tools, AI agents & developer automation

**Less setup. More building.**

I'm [Nimesh](https://github.com/npandeya). Nimesh Builds is where I build useful developer tools with AI and share the work in public: the design decisions, experiments, working demos, and lessons along the way.

[Explore the roadmap](https://github.com/nimeshbuilds/.github/blob/main/ROADMAP.md) · [Join the community](https://github.com/orgs/nimeshbuilds/discussions) · [Contribute](https://github.com/nimeshbuilds/.github/blob/main/CONTRIBUTING.md)

## Replicove: Kubernetes replica environments

<img src="https://raw.githubusercontent.com/nimeshbuilds/replicove/main/assets/brand/replicove-icon.png" alt="Replicove Kubernetes replica operator" width="80">

**Your cluster’s tools. A fresh place to test.**

[Replicove](https://github.com/nimeshbuilds/replicove) is an open-source Kubernetes operator for disposable integration environments powered by [vCluster](https://www.vcluster.com/). Select the operators, Helm components, configuration, and explicitly granted secrets your application needs, customize the selection, and request a replica with a Kubernetes manifest.

- **Provision:** install Replicove with one Helm command, then create new vClusters on demand or use an explicitly registered existing guest.
- **Reproduce:** apply selected components with namespace mappings, overrides, dependency planning, and optional plan approval.
- **Connect:** issue temporary guest credentials for developers, CI, and agents.
- **Clean up:** expire replicas with a TTL and verify cleanup of recorded resources while preserving sources and independently managed runtimes.

**Status: experimental alpha.** The [v0.1.0-alpha.1 release](https://github.com/nimeshbuilds/replicove/releases/tag/v0.1.0-alpha.1) includes public amd64/arm64 operator images, an OCI Helm chart, native YAML, and macOS/Linux CLI downloads. Disposable-cluster tests cover the new/existing vCluster paths and small cert-manager, Spark, Trino, and admission-policy scenarios. Production certification, cloud identity, and source volume data restoration remain future work.

→ [Install with Helm](https://nimeshbuilds.github.io/replicove/getting-started/helm/) · [Developer documentation](https://nimeshbuilds.github.io/replicove/) · [Explore the code](https://github.com/nimeshbuilds/replicove)

## What you'll find here

| Area | Problems we want to solve |
| --- | --- |
| Kubernetes & platform engineering | Reproducible development environments, integration testing, and operator setup. |
| AI agents & automation | Useful coordination, evaluation, and repeatable developer workflows. |
| Developer tools | Small tools that remove everyday setup and maintenance work. |

## Build with me

- **Have a real problem?** Start an [Ideas discussion](https://github.com/nimeshbuilds/.github/discussions/categories/ideas) with the workflow, what hurts, and what you've tried.
- **Want to contribute?** Review a design, improve the docs, or pick a scoped task from the [community issues](https://github.com/nimeshbuilds/.github/issues).
- **Want updates?** Follow [@nimeshbuilds](https://github.com/nimeshbuilds) and watch the [Announcements](https://github.com/nimeshbuilds/.github/discussions/categories/announcements). Star individual projects when they're useful to you.

AI helps with the work. Maintainers remain responsible for review, evidence, and what ships.

---

[Contribution guide](https://github.com/nimeshbuilds/.github/blob/main/CONTRIBUTING.md) · [Community standards](https://github.com/nimeshbuilds/.github/blob/main/CODE_OF_CONDUCT.md) · [Get help](https://github.com/nimeshbuilds/.github/blob/main/SUPPORT.md) · [Report a vulnerability](https://github.com/nimeshbuilds/.github/blob/main/SECURITY.md)
