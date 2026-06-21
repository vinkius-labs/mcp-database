# Zuplo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zuplo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage API gateways, edge deployments, and consumers on Zuplo — the programmable API management platform for developers.

## Description
Connect your **Zuplo** account to any AI agent and manage your programmable API infrastructure through natural conversation.

### What you can do

- **Project Management** — List all Zuplo projects and API gateways in your account to monitor your integration landscape
- **Edge Deployments** — Trigger new configuration deployments to the global edge network or audit previous deployment history
- **Consumer Governance** — Create, manage, and revoke API key consumers to control who has access to your gateway authentication
- **Environment Auditing** — List available project environments (e.g., working, production) and verify their current operational status
- **DNS & Domains** — Retrieve and manage configured custom DNS domains for each of your API projects directly from your agent
- **Real-Time Metrics** — Monitor gateway traffic, latency, and throughput metrics directly from Zuplo's edge analytics network
- **Declarative Config** — Browse and list the configuration files that define your gateway's routing and policy logic

### How it works

1. Subscribe to this server
2. Enter your Zuplo API Key
3. Start managing your API gateways through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex cloud consoles to whitelist a consumer. Your AI agent becomes your API platform engineer.

### Who is this for?

- **Platform Engineers** — monitor edge metrics and manage consumer identities through simple chat commands
- **API Developers** — trigger deployments and audit configuration files without manual data entry
- **DevOps Teams** — verify environment health and monitor custom domain configurations through conversation
- **Security Architects** — audit API key consumers and manage gateway authentication policies rapidly


## Available Tools
- **list_consumers**: List API key consumers
- **create_consumer**: Create API key consumer
- **create_deployment**: Create a new deployment
- **delete_consumer**: Delete API key consumer
- **list_custom_domains**: List custom domains
- **list_environments**: g., working, production) for a Project.

List project environments
- **list_files**: List configuration files
- **list_deployments**: List deployments
- **get_metrics**: Get edge metrics
- **list_projects**: List Zuplo projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zuplo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zuplo projects."

**🤖 AI Agent:**
> I found 3 Zuplo projects: 1. 'Payment-Gateway-Main' (ID: proj-101), 2. 'User-Auth-Edge' (ID: proj-102), and 3. 'Legacy-API-Proxy' (ID: proj-103). Which one would you like to see metrics for?

---

**👤 You:**
> "Check the latency metrics for 'proj-101'."

**🤖 AI Agent:**
> Latency metrics for proj-101: Average p95 latency is 42ms. Total traffic in the last 24h: 1.2 million requests. Current error rate: 0.05%. Everything looks healthy across the edge network.

---

**👤 You:**
> "Create a new consumer for 'Acme Partner' in project 'proj-101'."

**🤖 AI Agent:**
> Success! I've provisioned a new consumer identity for 'Acme Partner' (ID: cons-999) in project proj-101. I can provide the associated API key details if you need them for delivery.


## ❓ FAQ

**Q: Can I check my API gateway metrics through the agent?**
Yes. The `get_metrics` tool allows your AI agent to retrieve real-time traffic and latency data for any specific project ID, helping you monitor gateway performance directly through chat.

**Q: How do I create a new consumer identity for API key authentication?**
You can use the `create_consumer` tool. Provide the project ID and a JSON payload with the consumer's details, and Zuplo will provision the new identity for your API gateway instantly.

**Q: Is it possible to see my project's configuration files via conversation?**
Absolutely. Use the `list_project_files` tool to retrieve the declarative configuration files for your API project, allowing you to audit routing and policy definitions through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zuplo](https://vinkius.com/mcp/zuplo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zuplo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zuplo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zuplo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zuplo": {
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
