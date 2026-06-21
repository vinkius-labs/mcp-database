# Kubernetes Architecture Prover MCP Server

An AI generated Kubernetes manifests for a payment service. No resource requests or limits. No PodSecurityStandards. Single replica, no PDB. Zero NetworkPolicies — every pod could reach every other pod. The payment pod got OOM-killed at 3 AM by a logging sidecar with no memory ceiling. This tool forces resource governance, security hardening, reliability design, observability instrumentation, and network restriction on every workload.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kubernetes-architecture-prover)

## Overview
**Category:** infrastructure
**Tools Count:** 1

## Description
AI agents generate Kubernetes manifests that deploy successfully — until they cause production outages. They skip resource requests and limits. They run containers as root. They deploy single-replica services with no disruption budgets. They configure zero NetworkPolicies — flat L3 means a compromised pod reaches everything. They skip probes entirely. The deployment works. The architecture is a liability.

### The Problem

LLMs commit five Kubernetes architecture failures that compound in production:

- **Resource Anarchy** — No requests, no limits, no LimitRanges, no ResourceQuotas. A logging sidecar with no memory ceiling OOM-kills the payment service at 3 AM. The node runs out of allocatable capacity. Pods get evicted by priority — and yours has none set.
- **Security Theater** — Containers run as root. No PodSecurityStandards enforced. Capabilities not dropped. hostPID and hostNetwork enabled 'for debugging.' A container escape gives the attacker node-level access.
- **Single Point of Failure** — One replica. No PodDisruptionBudget. No anti-affinity. A node drain during maintenance takes down the service. Rolling updates with maxUnavailable=1 on a single replica mean zero availability during deploy.
- **Blind Operations** — No liveness probe — Kubernetes cannot detect deadlocks. No readiness probe — traffic routes to unready pods. No structured logging — 'kubectl logs' across 40 pods at 3 AM. No metrics — you learn about failures from users.
- **Flat Networking** — No NetworkPolicies. Every pod can reach every other pod on every port. No ingress TLS termination. No egress restrictions. A compromised pod scans the entire cluster and exfiltrates data over any port.

### How It Works

Kubernetes Architecture Prover validates workload architecture through 5 Decision Pivots:

1. **resourcesGoverned** — CPU/memory requests AND limits on every container. LimitRanges for namespace defaults. ResourceQuotas for namespace ceilings. Not 'the cluster handles it.'
2. **securityHardened** — runAsNonRoot=true, runAsUser≥1000, PodSecurityStandard baseline/restricted, drop ALL capabilities, readOnlyRootFilesystem=true, no hostPID/hostNetwork. Not 'behind a firewall.'
3. **reliabilityDesigned** — ≥2 replicas for production, PodDisruptionBudget with minAvailable, anti-affinity across nodes/zones, HPA or VPA autoscaling. Not 'Kubernetes restarts pods.'
4. **observabilityInstrumented** — Liveness probe (deadlock detection), readiness probe (traffic gating), startup probe (slow boot), structured JSON logging aggregated centrally, Prometheus metrics with SLO-based alerting. Not 'we check the dashboard.'
5. **networkingRestricted** — Deny-all default NetworkPolicies with explicit allow rules, ingress TLS via cert-manager, egress whitelist, mTLS between services. Not 'flat network is simpler.'

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| resourcesGoverned = false | RESOURCES_UNGOVERNED | No limits. Noisy neighbors will OOM-kill your workloads. |
| securityHardened = false | SECURITY_UNHARDENED | Running as root. Container escape = node compromise. |
| reliabilityDesigned = false | RELIABILITY_UNDESIGNED | Single replica. Node drain = full outage. |
| observabilityInstrumented = false | OBSERVABILITY_ABSENT | No probes, no metrics. You find out from users. |
| networkingRestricted = false | NETWORKING_EXPOSED | Flat L3. Compromised pod reaches everything. |
| All pivots pass | ARCHITECTURE_PROVEN | Governed, hardened, reliable, observable, restricted. |

### Why It Works

- **Tool calls are obligations.** The agent cannot skip resource definitions or claim security without specifying runAsUser and PodSecurityStandard. Filling the fields IS the architecture work.
- **Consistency engine catches contradictions.** If the agent claims `securityHardened=true` but mentions 'containers need root for setup,' the engine rejects with a specific coaching message.
- **Semantic traps detect hand-waving.** Phrases like 'the cluster handles it,' 'Kubernetes restarts pods,' or 'flat network is simpler' trigger automatic rejection. Name the value. Name the policy. Name the probe endpoint.


## Available Tools
- **validate_kubernetes_architecture**: Kubernetes gives you power without guardrails — every guardrail must be explicitly configured. You must: (1) define RESOURCE GOVERNANCE — CPU/memory requests AND limits for every container, LimitRanges per namespace for defaults, ResourceQuotas for namespace ceilings. "The cluster handles it" is not governance, (2) enforce SECURITY HARDENING — runAsNonRoot, drop ALL capabilities, readOnlyRootFilesystem, PodSecurityStandard restricted, signed images, no :latest tag. Root containers inherit node-level attack surface, (3) design RELIABILITY — ≥2 replicas for production, PodDisruptionBudgets, anti-affinity across zones, HPA/VPA autoscaling. Single-replica = zero redundancy during drain, (4) instrument OBSERVABILITY — liveness, readiness, and startup probes with correct timing. Structured JSON logging aggregated to a central system. Prometheus metrics with SLO-based alerting. "We check the logs" is not observability, (5) restrict NETWORKING — default deny-all NetworkPolicies with explicit allow rules. Ingress TLS via cert-manager. Egress whitelists. mTLS between services. Flat network = any compromised pod reaches everything. If rejected, fix the specific architecture gap.

Structured reflection tool for production Kubernetes architecture — forces resource governance, security hardening, reliability design, observability instrumentation, and network restriction before any workload reaches production. Catches Resources Ungoverned (deploying containers without CPU/memory requests and limits — "the cluster handles it" is not governance. Without requests, the scheduler cannot make informed decisions — it places pods on nodes that may already be overcommitted. Without limits, a single memory-leaking container consumes the entire node, evicting all other pods. Without LimitRanges, any developer can request 64GB RAM. Without ResourceQuotas, one namespace can starve others. "100m/500m CPU, 128Mi/512Mi memory per container, LimitRange 2Gi max, ResourceQuota 16Gi/namespace" is governance), Security Unhardened (running containers as root with full capabilities — a root container with NET_RAW capability can ARP-spoof the entire node network. runAsNonRoot=true, runAsUser≥1000, drop ALL capabilities, readOnlyRootFilesystem=true, PodSecurityStandard=restricted. "We trust our images" is not security — a compromised dependency in any base image inherits root privileges), Reliability Undesigned (single-replica production workloads without disruption budgets — Kubernetes drains nodes for upgrades. A single-replica workload has zero redundancy during drain. PodDisruptionBudget with minAvailable=1, anti-affinity across zones, HPA scaling 2→10 based on CPU. "It restarts fast" is not reliability — restart means downtime), Observability Absent (no probes, no structured logging, no metrics, no SLO alerting — without a readiness probe, Kubernetes sends traffic to pods that are not ready to serve. Without a liveness probe, a deadlocked pod is never restarted. Without startup probes, slow-boot JVM containers get killed before initialization. "We check the logs" is not observability — structured JSON logging, Prometheus metrics, and SLO-based alerting (error budget burn rate) is observability), and Networking Exposed (flat network with no network policies — in a flat Kubernetes network, any pod can reach any other pod on any port. A compromised frontend pod can directly query the database pod. Default deny-all NetworkPolicy per namespace, explicit ingress/egress allow rules per service, mTLS between services via service mesh. "We use private subnets" is not network security inside a cluster). Call once per Kubernetes deployment or architecture review


## Installation & Usage

To install and use the **Kubernetes Architecture Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kubernetes-architecture-prover](https://vinkius.com/mcp/kubernetes-architecture-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
