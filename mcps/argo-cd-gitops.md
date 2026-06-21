# Argo CD (GitOps) MCP Server

Manage Kubernetes deployments via Argo CD — sync applications, check logs, and manage clusters/repositories directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/argo-cd-gitops)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

## Description
Connect your **Argo CD** instance to any AI agent and take full control of your GitOps workflows through natural conversation.

### What you can do

- **Application Lifecycle** — List all deployed applications, trigger sync operations, and perform rollbacks to previous stable versions.
- **Observability** — Fetch real-time logs for specific applications to debug deployment issues without leaving your terminal or chat interface.
- **Project Management** — List and inspect AppProjects to understand logical groupings, permissions, and resource constraints.
- **Infrastructure Control** — Manage target clusters and Git/Helm repositories registered in your Argo CD environment.
- **Cluster Operations** — Add or remove Kubernetes clusters to scale your deployment targets dynamically.

### How it works

1. Subscribe to this server
2. Enter your Argo CD Server URL and Auth Token
3. Start managing your Kubernetes clusters from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly sync apps and check deployment health across multiple clusters.
- **SREs** — investigate production issues by pulling application logs directly into the AI context for analysis.
- **Software Developers** — manage their own application environments and roll back changes without needing deep CLI knowledge.


## Available Tools
- **add_cluster**: Add a new cluster to Argo CD
- **add_repository**: Add a new repository to Argo CD
- **get_application_logs**: Get logs for an Argo CD application
- **create_application**: Create a new Argo CD application
- **create_project**: Create a new Argo CD project
- **delete_cluster**: Delete a cluster from Argo CD
- **get_project**: Get details for a specific Argo CD project
- **list_applications**: List Argo CD applications
- **list_clusters**: List Argo CD clusters
- **list_projects**: List Argo CD projects
- **list_repositories**: List Argo CD repositories
- **rollback_application**: Rollback an Argo CD application
- **sync_application**: Sync an Argo CD application


## Installation & Usage

To install and use the **Argo CD (GitOps)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argo-cd-gitops](https://vinkius.com/mcp/argo-cd-gitops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
