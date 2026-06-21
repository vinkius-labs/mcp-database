# Papertrail (Real-time Cloud Log Manager) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/papertrail-real-time-cloud-log-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Manage and analyze cloud logs in real-time via Papertrail — search events, list systems, and organize log groups directly from your AI agent.

## Description
Connect **Papertrail** to your AI agent for instant visibility into your cloud infrastructure logs and real-time troubleshooting through natural conversation.

### What you can do

- **Event Searching** — Search through millions of log events using Papertrail's powerful search syntax, with support for pagination and live tailing.
- **System Monitoring** — List all systems currently sending logs to your account to ensure your infrastructure is reporting correctly.
- **Group Organization** — List and create log groups to categorize your systems and streamline your monitoring workflows.
- **Destination Management** — View and configure log destinations to control where your data is archived or forwarded.
- **Real-time Debugging** — Quickly identify errors and performance bottlenecks by querying logs directly from your development environment.

### How it works

1. Subscribe to this server
2. Enter your Papertrail API Token
3. Start searching logs and managing systems from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — monitor system health and troubleshoot production issues without leaving the terminal or chat interface
- **Backend Developers** — search for specific error traces and debug API issues directly from the code editor
- **System Administrators** — manage log groups and destinations to maintain a clean and organized logging infrastructure


## Available Tools
- **create_destination**: Create a new log destination
- **create_group**: Create a new log group
- **list_destinations**: List log destinations
- **list_groups**: List all log groups
- **search_events**: Search through log events
- **list_systems**: List all systems sending logs to Papertrail


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Papertrail (Real-time Cloud Log Manager)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all systems sending logs to my Papertrail account."

**🤖 AI Agent:**
> I've retrieved your systems. You have 3 active systems: 'web-prod-01' (ID: 101), 'db-master' (ID: 102), and 'api-gateway' (ID: 103).

---

**👤 You:**
> "Search for 'ConnectionTimeout' in the logs."

**🤖 AI Agent:**
> Searching events... I found 12 occurrences of 'ConnectionTimeout' in the last hour. Most are coming from 'api-gateway'. Would you like to see the full log entries?

---

**👤 You:**
> "Create a new log group called 'Critical-Services' for systems 101 and 103."

**🤖 AI Agent:**
> Successfully created the log group 'Critical-Services' (ID: 505) containing systems 101 and 103. You can now filter searches specifically for this group.


## ❓ FAQ

**Q: Can I search for specific error messages across all my logs?**
Yes! Use the `search_events` tool with the `q` parameter. You can use Papertrail's search syntax (e.g., 'error OR critical') to filter events across your systems.

**Q: How do I see which servers or applications are currently sending logs?**
Simply run the `list_systems` tool. It will return a list of all systems configured in your Papertrail account, including their names and IDs.

**Q: Can I create a new group to organize specific systems?**
Yes, use the `create_group` tool. You can provide a name and a comma-separated list of system IDs to group them together for easier monitoring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/papertrail-real-time-cloud-log-manager](https://vinkius.com/mcp/papertrail-real-time-cloud-log-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Papertrail (Real-time Cloud Log Manager)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `papertrail-real-time-cloud-log-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Papertrail (Real-time Cloud Log Manager)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "papertrail-real-time-cloud-log-manager": {
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
