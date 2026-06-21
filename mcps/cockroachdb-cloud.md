# CockroachDB Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cockroachdb-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage distributed SQL clusters via CockroachDB Cloud — track clusters, monitor nodes, and audit network allowlists directly from any AI agent.

## Description
Connect your **CockroachDB Cloud** account to any AI agent and take full control of your distributed SQL infrastructure through natural conversation. Streamline how you monitor and manage your globally-scalable databases natively.

### What you can do

- **Cluster Oversight** — List and retrieve details for all CockroachDB Cloud clusters including provider and region info natively
- **Node Intelligence** — Access and monitor individual nodes within your clusters to understand health and status flawlessly
- **Operation Auditing** — List and review recent management operations like scaling or upgrades to track changes securely
- **Network Logistics** — Access and monitor network allowlist rules to ensure secure database connectivity flawlessly
- **Encryption Management** — List Customer Managed Keys (CMKs) used for cluster-level data encryption flawlessly
- **Account Visibility** — Retrieve information about your authenticated user profile and organization directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CockroachDB Cloud API Secret Key
3. Start managing your distributed databases from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Database Administrators (DBAs)** — monitor cluster health and operation history using natural language
- **Cloud Engineers** — audit network allowlists and regional distribution without opening the cloud console
- **Security Teams** — quickly look up encryption key metadata and connectivity rules straight from their chat interface
- **Platform Teams** — verify cloud provider availability and monitor cluster lifecycle events


## Available Tools
- **get_cluster_cloud_details**: Get detailed information for a specific cluster
- **get_my_cockroach_profile**: Retrieve information about the authenticated user/organization
- **list_network_allowlist**: List network allowlist rules for a specific cluster
- **list_encryption_keys**: List Customer Managed Keys (CMKs) used for cluster encryption
- **list_supported_cloud_providers**: List cloud providers supported by CockroachDB Cloud
- **list_cockroach_clusters**: List all CockroachDB Cloud clusters
- **list_cluster_nodes**: List all nodes within a specific cluster
- **list_cluster_operations**: List recent management operations for a cluster (e.g. scaling, upgrades)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CockroachDB Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my CockroachDB clusters."

**🤖 AI Agent:**
> Retrieving your database clusters... I found 2 clusters: 'Production-Main' (AWS, us-east-1) and 'Dev-Sandbox' (GCP, europe-west1). Both are currently in 'RUNNING' status.

---

**👤 You:**
> "Show me the network allowlist for the 'Production-Main' cluster."

**🤖 AI Agent:**
> Checking network allowlist... The Production-Main cluster has 3 rules: 'Office VPN' (1.2.3.4/32), 'App Server Fleet' (10.0.0.0/16), and 'Admin Backup' (5.6.7.8/32).

---

**👤 You:**
> "What was the result of the last operation on cluster 'Dev-Sandbox'?"

**🤖 AI Agent:**
> Retrieving last operation... The most recent task was 'CLUSTER_UPDATE' (minor version upgrade) completed successfully two hours ago. It took approximately 15 minutes.


## ❓ FAQ

**Q: Can I see the status of all nodes in a cluster through the agent?**
Yes! Use the `list_cluster_nodes` tool with the unique cluster ID. The agent will return a list of all nodes, their IP addresses, and their current health/operational state.

**Q: How do I check for recent scaling or upgrade events on my database?**
Use the `list_cluster_operations` tool. Your agent will fetch the management log for the cluster, showing you recent tasks, their progress, and whether they were successful.

**Q: Where do I find my CockroachDB Cloud API Secret Key?**
Log in to the CockroachDB Cloud Console, navigate to **Access Management**, and select **API Keys**. You can generate and copy a new Secret Key from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cockroachdb-cloud](https://vinkius.com/mcp/cockroachdb-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CockroachDB Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cockroachdb-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CockroachDB Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cockroachdb-cloud": {
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
