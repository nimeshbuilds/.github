<p align="center">
  <img src="https://raw.githubusercontent.com/nimeshbuilds/.github/main/assets/banner.png" alt="Nimesh Builds — Vibe coding. Open source. Built in public." width="100%">
</p>

# Open-source Kubernetes tools, AI agents & developer automation

**Less setup. More building.**

I'm [Nimesh](https://github.com/npandeya). Nimesh Builds is where I build useful developer tools with AI and share the work in public: the design decisions, experiments, working demos, and lessons along the way.

[Explore the roadmap](https://github.com/nimeshbuilds/.github/blob/main/ROADMAP.md) · [Join the community](https://github.com/orgs/nimeshbuilds/discussions) · [Contribute](https://github.com/nimeshbuilds/.github/blob/main/CONTRIBUTING.md)

## First project: ClusterReplica

**Recreate the Kubernetes toolset you need in an ephemeral vCluster.**

Integration tests need more than an empty cluster. They need the operators, configuration, and dependencies your application actually uses.

ClusterReplica is a planned Kubernetes operator that wraps [vCluster](https://www.vcluster.com/) to make that setup easier. The goal: request a development cluster with one custom resource, select what to reproduce from the host, customize it, and let it expire when the work is done.

The proposed workflow covers:

- **Provision:** create a vCluster or use an explicitly selected existing one.
- **Reproduce:** install supported operators and selected configuration, with overrides.
- **Connect:** provide scoped access for developers, CI jobs, and agents.
- **Clean up:** expire the environment with a TTL and track deletion of owned resources.

**Status: design and validation.** There is no released operator, installation command, or certified compatibility matrix yet. Kubernetes versions and required capabilities will determine support; cloud identity, storage, secrets, and operator behavior need explicit validation.

→ [Read the project brief](https://github.com/nimeshbuilds/.github/blob/main/projects/cluster-replica.md) · [Share your cluster-testing pain points](https://github.com/nimeshbuilds/.github/discussions/categories/ideas)

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
