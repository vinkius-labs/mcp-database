# Argo Workflows MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/argo-workflows)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate Kubernetes orchestrations via Argo Workflows — monitor, list, and inspect active pods, crons, and workflow templates directly from any AI agent.

## Description
Connect your **Argo Workflows** cluster to any AI agent and take full control of your infrastructure orchestration through natural conversation.

### What you can do

- **Active Workflows** — List and query all running, pending, or recently completed workflow executions across your Kubernetes namespaces
- **Deep Inspection** — Dive into specific workflow instances to inspect their precise resource trees, node statuses, and pod parameters to catch failures
- **Templates & Crons** — Browse parameterized, reusable WorkflowTemplates and analyze recurring CronWorkflows orchestrating scheduled jobs
- **Historical Archives** — Search archived workflows that hit your database to understand historical infrastructure patterns

### How it works

1. Subscribe to this server
2. Enter your Argo Cluster Server URL and RBAC Bearer Token
3. Start querying your execution trees from Claude, Cursor, or any MCP-compatible client

No more wrestling with `kubectl` CLI tools or constantly refreshing the Argo Web UI to find out why a step failed. Your AI acts as your ultimate DevOps copilot.

### Who is this for?

- **DevOps & Platform Teams** — debug pipeline failures, check node statuses, and audit running jobs without leaving your terminal or chat workflow
- **Data Engineers** — monitor complex ETL workflows and scheduled cron operations seamlessly
- **SREs** — quickly query the health of the Argo server and retrieve historical archiving metrics


## Available Tools
- **list_workflows**: List workflows in a Kubernetes namespace
- **get_workflow**: Get detailed resource tree and status for an Argo workflow
- **list_workflow_templates**: List workflow templates defined in a namespace
- **list_cron_workflows**: List scheduled cron workflows in a namespace
- **list_archived_workflows**: List archived workflows from Argo history
- **get_server_info**: Get Argo Workflows server information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Argo Workflows** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workflows in the 'data-engineering' namespace."

**🤖 AI Agent:**
> I found 4 active workflows in 'data-engineering'. Three are executing robustly, but 'etl-nightly-pipeline' has been pending for 22 minutes. Would you like me to get the deep tree view of this pipeline to see which pod is stuck?

---

**👤 You:**
> "What is the detailed status tree of the workflow named 'daily-backup-55x'?"

**🤖 AI Agent:**
> I've inspected the tree for 'daily-backup-55x'. The master process reports 'Failed'. Specifically, node 's3-upload-step' crashed exiting with code 1. The previous node 'pg-dump' succeeded. It seems to be an S3 permission issue in the pod parameter payload.

---

**👤 You:**
> "Are there any parameterized WorkflowTemplates available for me to run?"

**🤖 AI Agent:**
> Listing your templates... You have 3 reusable components: `model-training-tmpl` (requires hyperparameters as array input), `data-cleanup` (expects an S3 bucket URI), and `slack-notification-hook`. They are all initialized and stored in the default namespace.


## ❓ FAQ

**Q: Can my AI agent figure out exactly which pod/node failed in an active workflow execution?**
Yes. If a workflow fails, you can ask your agent to retrieve the workflow tree by name. The agent uses the `get_workflow` tool to inspect the deeply nested structure, traverse the active nodes, and pinpoint the exact step or container that resulted in an error state without you ever needing to click through the Argo UI.

**Q: Can I list only scheduled periodic jobs across my cluster?**
Absolutely. You can use the dedicated `list_cron_workflows` capability to isolate and return strictly workloads orchestrated on a time schedule across any namespace, saving you from parsing through thousands of isolated runs.

**Q: Do I need to expose my internal Kubernetes API to use this?**
No. The integration strictly interfaces with the Argo Server UI/API layer via standard REST traffic using a scoped ServiceAccount Bearer token. Your cluster's overarching master `kube-apiserver` remains safely isolated from external agentic logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argo-workflows](https://vinkius.com/mcp/argo-workflows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Argo Workflows** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `argo-workflows` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Argo Workflows** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "argo-workflows": {
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
