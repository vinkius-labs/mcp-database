# Argo CD (GitOps) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/argo-cd-gitops)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/argo-cd-gitops-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/argo-cd-gitops-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Kubernetes deployments via Argo CD — sync applications, check logs, and manage clusters/repositories directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Argo CD (GitOps)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications currently managed in Argo CD."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'guestbook' (Healthy), 'helm-guestbook' (Synced), and 'staging-api' (OutOfSync). Would you like to sync 'staging-api'?

---

**👤 You:**
> "Sync the application named 'production-backend'."

**🤖 AI Agent:**
> Initiating sync for 'production-backend'... The operation was successful. The application is now progressing towards a Synced and Healthy state.

---

**👤 You:**
> "Show me the logs for the 'frontend-app' to see why it's crashing."

**🤖 AI Agent:**
> Fetching logs for 'frontend-app'... I see a recurring 'Back-off restarting failed container' error. The last log entry indicates a connection timeout to the database service. Should I check the database application status?


## Installation & Usage

To install and use the **Argo CD (GitOps)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argo-cd-gitops](https://vinkius.com/mcp/argo-cd-gitops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
