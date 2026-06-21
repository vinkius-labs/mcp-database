# Kubernetes Architecture Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kubernetes-architecture-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

An AI generated Kubernetes manifests for a payment service. No resource requests or limits. No PodSecurityStandards. Single replica, no PDB. Zero NetworkPolicies — every pod could reach every other pod. The payment pod got OOM-killed at 3 AM by a logging sidecar with no memory ceiling. This tool forces resource governance, security hardening, reliability design, observability instrumentation, and network restriction on every workload.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kubernetes Architecture Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Deploy a Node.js API to Kubernetes. Use the default settings, one replica should be enough. We will add monitoring later."

**🤖 AI Agent:**
> RESOURCES_UNGOVERNED — 'Default settings' means no CPU/memory requests or limits. The first noisy neighbor OOM-kills your API. Define: [API container: CPU 100m/500m, memory 128Mi/512Mi] → [LimitRange: default 100m CPU, 128Mi memory] → [ResourceQuota: 2 CPU, 2Gi memory ceiling]. Also: single replica + no monitoring = blind single point of failure.

---

**👤 You:**
> "API container: CPU 200m/1000m, memory 256Mi/1Gi. LimitRange: default 100m/128Mi. ResourceQuota: 8 CPU, 16Gi. Security: runAsNonRoot=true, runAsUser=1001, PodSecurityStandard=restricted, drop ALL capabilities, readOnlyRootFilesystem=true. Reliability: 3 replicas, PDB minAvailable=2, podAntiAffinity on topology.kubernetes.io/zone, HPA targeting 70% CPU, min=3 max=10. Observability: liveness GET /healthz initialDelay=15s period=10s, readiness GET /ready failureThreshold=3, startup GET /healthz failureThreshold=30 period=10s, structured JSON logging to Loki, Prometheus /metrics endpoint with p99 latency alerting at 500ms SLO. Networking: deny-all default NetworkPolicy, allow ingress from nginx-ingress namespace on port 3000, allow egress to postgres on port 5432 and to external API on port 443, TLS via cert-manager with Let's Encrypt, Linkerd mTLS between services."

**🤖 AI Agent:**
> ARCHITECTURE_PROVEN — Production-grade Kubernetes architecture validated. Resources: 200m/1Gi with namespace governance. Security: restricted PSS, non-root, capabilities dropped. Reliability: 3 replicas across zones with PDB and HPA. Observability: full probe chain, Loki logging, Prometheus with p99 SLO alerting. Networking: deny-all with explicit allow, cert-manager TLS, Linkerd mTLS. This workload survives node failure, maintenance drain, and lateral movement attempts.

---

**👤 You:**
> "Resources: CPU 100m/500m per container, LimitRange set, ResourceQuota 4CPU/8Gi. Security: runAsNonRoot=true, restricted PSS. Reliability: 2 replicas, PDB minAvailable=1, anti-affinity on hostname. Observability: liveness and readiness probes configured, logs to stdout. But we keep the default flat network because all our services need to communicate with each other and NetworkPolicies add complexity."

**🤖 AI Agent:**
> NETWORKING_EXPOSED — Resources, security, reliability, and observability pass — but networking is flat. 'All services need to communicate' is false — your API does not need to reach your monitoring stack's database. Define deny-all default policies, then allow only the specific pod-to-pod flows you need. 'NetworkPolicies add complexity' — so does a compromised pod scanning your entire cluster. Also: 'logs to stdout' without structured format or aggregation target is insufficient observability.


## ❓ FAQ

**Q: Does it generate Kubernetes manifests?**
No. It validates that your architecture addresses the five production-critical pillars — resource governance, security hardening, reliability design, observability instrumentation, and network restriction. It does not generate YAML. It forces you to prove your YAML is production-ready.

**Q: What counts as proper resource governance?**
Every container must have CPU and memory requests AND limits. Every namespace must have a LimitRange (defaults for containers that don't specify) and a ResourceQuota (ceiling for the namespace). 'The cluster handles it' is not governance — it is the absence of governance.

**Q: Is it useful for managed Kubernetes (EKS, GKE, AKS)?**
Yes. Managed Kubernetes handles the control plane — it does NOT handle your workload architecture. Resource limits, security context, PDBs, probes, and NetworkPolicies are YOUR responsibility on every provider. The cloud provider manages etcd. You manage everything that runs on the nodes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kubernetes-architecture-prover](https://vinkius.com/mcp/kubernetes-architecture-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kubernetes Architecture Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kubernetes-architecture-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kubernetes Architecture Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kubernetes-architecture-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
