# Porter PaaS MCP Server

Orchestrate Kubernetes clusters via Porter — manage apps, projects, container tags, and enforce rollouts directly with your AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/porter-paas)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Porter PaaS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/porter-paas](https://vinkius.com/mcp/porter-paas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
