# ClientSuccess MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientsuccess-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clientsuccess-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clientsuccess-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Reduce churn and grow accounts with health scoring, engagement tracking, and success playbooks built for customer success teams.

## Description
Connect your **ClientSuccess** customer success platform to any AI agent and simplify how you manage your client relationships, track account health, and monitor service contracts through natural conversation.

### What you can do

- **Client Oversight** — List all managed clients and retrieve detailed metadata, including health scores and success status.
- **Relationship Management** — Manage client contacts, query individual profiles, and create new client records programmatically.
- **Contract Monitoring** — List active and historic service contracts to ensure your renewals and agreements are on track.
- **Segmentation** — Query customer segments to understand your client distribution and categorization.
- **Data Insights** — Fetch complete account metadata and health metrics to identify at-risk customers via AI.
- **Operational Efficiency** — Track your customer success ecosystem directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your ClientSuccess API Key (found in your account settings)
3. Start managing your client relationships from your favorite AI assistant

### Who is this for?

- **Customer Success Managers (CSMs)** — quickly check client health scores and retrieve contact info via simple AI commands.
- **Success Operations** — monitor contract distributions and verify segment metadata directly from the workspace.
- **Product & Leadership Teams** — get instant bird's-eye views of client status and account growth via the AI assistant.


## Available Tools
- **create_client**: Create a new client
- **get_client_details**: Get details for a specific client
- **list_clients**: List ClientSuccess clients
- **list_contacts**: Optionally filter by client ID.

List client contacts
- **list_contracts**: List client contracts
- **list_segments**: List client segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClientSuccess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active clients in my ClientSuccess account."

**🤖 AI Agent:**
> I've retrieved your client directory. You have 35 active organizations including 'Acme Corp', 'Tech Giant', and 'Global Logistics'. Which one would you like to see the health score for?

---

**👤 You:**
> "Show me the details and health score for client 'Acme Corp' (ID: 10293)."

**🤖 AI Agent:**
> Fetching data... Acme Corp currently has a Health Score of 85/100 (Stable). They have 2 active contracts and their primary contact is Sarah Smith. Shall I retrieve their contract details?

---

**👤 You:**
> "List all my customer segments."

**🤖 AI Agent:**
> Retrieving segments... You have 5 segments configured: 'Enterprise', 'Mid-Market', 'SMB', 'Strategic Accounts', and 'Beta Testers'. Which segment would you like to explore?


## Installation & Usage

To install and use the **ClientSuccess** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientsuccess-alternative](https://vinkius.com/mcp/clientsuccess-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
