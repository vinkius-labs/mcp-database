# TiDB Cloud (Serverless Distributed SQL) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tidb-cloud-serverless-distributed-sql)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage TiDB Cloud infrastructure — list projects, inspect clusters, and monitor serverless instances directly from your AI agent.

## Description
Connect your **TiDB Cloud** account to any AI agent and manage your distributed SQL infrastructure through natural conversation.

### What you can do

- **Project Overview** — List all organizational projects and fetch metadata for specific environments to understand your resource allocation.
- **Instance Management** — Retrieve all TiDB X instances (including Starter, Essential, and Premium tiers) housed within your projects.
- **Dedicated Clusters** — List and inspect Dedicated clusters to get a clear view of your high-performance database topology.
- **Deep Metadata Access** — Fetch specific project details and IDs required for deeper infrastructure automation and monitoring.

### How it works

1. Subscribe to this server
2. Enter your TiDB Cloud Public and Private API Keys
3. Start managing your distributed databases from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Database Administrators** — quickly audit cluster distributions and project structures without navigating the web console.
- **Backend Engineers** — verify instance availability and project IDs directly from the coding environment.
- **DevOps Teams** — automate the discovery of cloud resources for documentation or status reporting.


## Available Tools
- **get_project**: Retrieve details for a specific project
- **list_clusters**: Retrieve all Dedicated clusters within a project
- **list_instances**: Retrieve all TiDB X instances within a project
- **list_projects**: List all accessible projects in your organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TiDB Cloud (Serverless Distributed SQL)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my TiDB Cloud projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Production-DB' (ID: 101), 'Staging-Env' (ID: 102), and 'Analytics-Data' (ID: 103). Which one would you like to inspect?

---

**👤 You:**
> "Show me all TiDB X instances in project 101."

**🤖 AI Agent:**
> In project 101, I found 2 instances: a 'Serverless Starter' instance in us-east-1 and a 'Premium' instance in eu-west-1. Both are currently running.

---

**👤 You:**
> "Get the details for dedicated clusters in project 103."

**🤖 AI Agent:**
> Checking dedicated clusters for project 103... I found one Dedicated cluster named 'Analytics-Main' with 3 TiKV nodes and 2 TiDB nodes. It is healthy and active.


## ❓ FAQ

**Q: Can I see both serverless and dedicated clusters with this server?**
Yes. Use `list_instances` to see TiDB X instances (Serverless/Starter/Premium) and `list_clusters` to view your Dedicated cluster infrastructure.

**Q: How do I get the ID of a specific project to query its instances?**
You can run the `list_projects` tool first. It will return a list of all accessible projects along with their unique IDs, which you can then use in `list_instances` or `list_clusters`.

**Q: Does this tool allow me to delete or create new clusters?**
No. The current version of the TiDB Cloud MCP server is focused on discovery and inspection (read-only operations) such as `list_projects`, `get_project`, and `list_clusters` to ensure safe infrastructure monitoring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tidb-cloud-serverless-distributed-sql](https://vinkius.com/mcp/tidb-cloud-serverless-distributed-sql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TiDB Cloud (Serverless Distributed SQL)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tidb-cloud-serverless-distributed-sql` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TiDB Cloud (Serverless Distributed SQL)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tidb-cloud-serverless-distributed-sql": {
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
