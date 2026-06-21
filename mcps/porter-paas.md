# Porter PaaS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/porter-paas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/porter-paas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/porter-paas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Orchestrate Kubernetes clusters via Porter — manage apps, projects, container tags, and enforce rollouts directly with your AI.

## Description
Connect your **Porter** account to any AI agent and take full programmatic control over your Kubernetes infrastructure natively.

### What you can do

- **Projects & Clusters** — List high-level organizational bounds, EKS/GKE clusters, and deployment zones
- **Applications & Environments** — Map staging/production namespaces, check active web services, and resolve container requirements
- **Operations** — Restart app pods gracefully or forcefully deploy specific image tags when resolving CI/CD breaks
- **Helm Inspections** — Check low-level Helm charts behind active components (like Postgres or Redis)

### How it works

1. Subscribe to this server
2. Enter your Porter API Token
3. Start managing your clusters straight from Claude, Cursor, or any MCP client

No pulling KUBECONFIG files, authenticating via cloud CLI tools, or navigating dashboards. Your orchestration lives in chat.

### Who is this for?

- **DevOps Engineers** — quickly restart crashing services and audit cluster architectures on the fly
- **Backend Developers** — rollback image tags and orchestrate quick deployments directly from standard chat
- **Engineering Leads** — inspect resource mapping and isolate distinct staging environments instantly


## Available Tools
- **deploy_app_tag**: Assigns a raw docker registry digest/tag directly causing Kubernetes to perform an absolute image pull orchestrating a fresh deployment state spanning replica boundaries.

Forcefully mutate the executed Docker image running internally
- **get_app**: Includes explicit CPU metrics requested, RAM limits mapped locally to the JVM/Node instances, and internal registry image hashes resolving at runtime.

Analyze architectural bindings orchestrating a specific App
- **get_cluster**: Inspect deep cloud credentials generating a specific K8s Cluster
- **get_project**: Perform structural extraction of metadata linked to a Porter Project
- **list_apps**: Discovers precisely which App routing identities expose `porter.run` subdomains or linked target custom apex mappings.

Inventory deployed discrete Applications mapping to a Cluster
- **list_clusters**: Exposes crucial execution zones hosting absolute memory nodes.

List underlying target cloud Kubernetes definitions bounds to Porter
- **list_environments**: Extract logic isolation environments overlapping the Cluster
- **list_projects**: Fetches indispensable integer `projectId` arrays coordinating everything strictly downstream inside AWS/GCP clusters.

Identify base Porter PaaS organizational scopes
- **list_helm_releases**: Vital for verifying if dependent third-party apps (e.g. Postgres databases or Metabase) deployed aside the primary stack succeeded during installation phases.

List underlying operational Helm configurations inside a namespace
- **restart_app**: Mandatory during severe connection leakage scenarios impacting native processes without modifying the fundamental code layer deployment tag.

Instruct the Kubernetes API to bounce the App deployment replicas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Porter PaaS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications currently running in cluster ID 5 on the Production environment."

**🤖 AI Agent:**
> I found 4 applications bound to the cluster namespace. We have `core-api`, `cron-sync-worker`, `redis-cache`, and `web-frontend`. The core API is serving on a porter.run subdomain mapping. Would you like me to get architectural configs for `core-api`?

---

**👤 You:**
> "The queue worker is completely hung. Please perform a forceful restart of the `async-worker` app."

**🤖 AI Agent:**
> Command received. I've sent the signal to recycle the pod replicas for `async-worker` across cluster 4. Kubernetes is now performing a rolling flush seamlessly. It will take roughly 15 seconds to stand out new instances and attach them.

---

**👤 You:**
> "We just built a hotfix on main. Deploy the image tag `d83a1b1` strictly onto `portal-frontend`."

**🤖 AI Agent:**
> I've successfully forced the container mutation! The `portal-frontend` application was patched to image tag `d83a1b1`. The cloud runner is pulling the fresh digest and orchestrating a replacement. Check the frontend in 1 minute.


## Installation & Usage

To install and use the **Porter PaaS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/porter-paas](https://vinkius.com/mcp/porter-paas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
