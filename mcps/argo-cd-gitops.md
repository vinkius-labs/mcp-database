# Argo CD (GitOps) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/argo-cd-gitops)
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


## ❓ FAQ

**Q: Can I trigger a manual synchronization for a specific application?**
Yes! Use the `sync_application` tool by providing the application name. The agent will trigger the Argo CD sync process and report the status back to you.

**Q: Is it possible to view application logs to debug a failing pod?**
Absolutely. The `get_application_logs` tool allows you to retrieve logs for any application managed by Argo CD, helping you identify issues directly within the conversation.

**Q: Can I manage the clusters connected to my Argo CD instance?**
Yes. You can use `list_clusters` to see all registered targets, `add_cluster` to register a new one, or `delete_cluster` to remove an existing server URL from your management plane.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argo-cd-gitops](https://vinkius.com/mcp/argo-cd-gitops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Argo CD (GitOps)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `argo-cd-gitops` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Argo CD (GitOps)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "argo-cd-gitops": {
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
