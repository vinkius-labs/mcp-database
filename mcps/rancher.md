# Rancher MCP Server

Equip your AI to manage Kubernetes environments directly through Rancher, overseeing clusters, namespaces, and active pods.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rancher)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Rancher** Kubernetes management platform to your AI agent, allowing seamless orchestration of your container infrastructure directly from a chat interface. By integrating this server, your AI can introspect and interact with multiple remote Kubernetes clusters managed governed by your Rancher deployment.

### What you can do

- **Cluster Oversight** — List and examine the status of all managed clusters connected to your Rancher control plane.
- **Namespace Discovery** — Explore specific logical partitions (namespaces) within those clusters without digging into complex kubectl configuration.
- **Workload Management** — Access deployments, daemonsets, and statefulsets to observe operational health across environments.
- **Pod Introspection** — Query individual pod states, find crashing containers, and pull context faster than running manual CLI queries.

### How it works

1. Enable the MCP server integration.
2. Configure it with your Rancher Server URL and the generated Bearer Token for API authentication.
3. Instruct your AI to inspect a cluster, query specific namespaces, or detail the status of a specific pod.

### Who is this for?

- **DevOps Engineers** — Debug and query live cluster statuses interactively, bypassing the need to constantly switch context between terminals and UI dashboards.
- **Kubernetes Administrators** — Run automated queries to verify policies, scaling sets, and general deployment topologies rapidly.
- **Backend Developers** — Ensure microservices are running smoothly on target clusters and verify namespace health without complex local setups.


## Available Tools
- **get_cluster**: Retrieves details for a specific Kubernetes cluster
- **get_project**: Retrieves details for a specific Rancher project
- **list_apps**: Lists Helm applications installed in a project
- **list_catalogs**: Lists available Helm chart repositories (Catalogs)
- **list_clusters**: Lists all Kubernetes clusters managed by Rancher
- **list_namespaces**: Lists Kubernetes namespaces associated with a project
- **list_nodes**: Lists all nodes within a specific cluster
- **list_projects**: Use this to find project IDs.

Lists logical projects within a cluster
- **list_users**: Lists all user accounts in the Rancher platform
- **list_workloads**: Lists all Kubernetes workloads (Deployments, StatefulSets) in a project


## Installation & Usage

To install and use the **Rancher** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rancher](https://vinkius.com/mcp/rancher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
