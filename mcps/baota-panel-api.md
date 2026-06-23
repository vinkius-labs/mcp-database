# Baota Panel / 宝塔面板 API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baota-panel-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Leading server management panel in China — manage websites, databases, and system resources via AI.

## Description
Empower your AI agent to orchestrate your server infrastructure with **Baota Panel** (宝塔面板), the dominant web hosting control panel in China. By connecting Baota to your agent, you transform complex server administration, website maintenance, and resource monitoring into a natural conversation. Your agent can instantly list managed websites, retrieve real-time system load, monitor database health, and even browse administrative logs without you ever needing to log in to the panel interface. Whether you are conducting a security audit or monitoring server performance, your agent acts as a real-time SRE assistant, keeping your infrastructure accurate and your services online.

### What you can do

- **Site Orchestration** — List and retrieve detailed information about all websites managed by your Baota Panel.
- **Resource Monitoring** — Get real-time system load, CPU usage, and RAM statistics to audit server health.
- **Database Management** — List all databases and retrieve metadata for your data storage infrastructure.
- **Operational Auditing** — Browse cron jobs, pending background tasks, and recent administrative logs.
- **Software Insights** — List installed software and plugins (Nginx, PHP, MySQL) to ensure your stack is up-to-date.

### How it works

1. Subscribe to this server
2. Enter your Panel Host, API Secret Key, and API ID
3. Ensure your caller IP is whitelisted in the Baota Panel settings
4. Start managing your server through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Server Administrators** — monitor system resources and coordinate maintenance through natural language queries.
- **Web Developers** — manage site configurations and audit database lists directly from your AI-powered workspace.
- **DevOps Engineers** — oversee cron tasks and monitor network traffic via a unified AI interface.
- **Baota Power Users** — integrate your existing server workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_disk_info**: Get disk usage
- **get_network_info**: Get network status
- **get_software_list**: ).

List installed software
- **get_system_total**: Get system load info
- **get_task_count**: Get pending task count
- **list_cron_tasks**: List cron jobs
- **list_databases**: List databases
- **list_ftp**: List FTP accounts
- **list_logs**: List panel logs
- **list_sites**: List websites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baota Panel / 宝塔面板 API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the system resource usage on my server."

**🤖 AI Agent:**
> I've retrieved the system load. CPU usage is currently at 15%, RAM usage is 45%, and the load average is 0.5. Your server is operating well within normal limits.

---

**👤 You:**
> "List all websites managed by Baota."

**🤖 AI Agent:**
> I've retrieved your websites from Baota Panel. You have 5 active sites, including 'marketing-landing.com' and 'api-server.net'. Would you like more details for any of them?

---

**👤 You:**
> "Show me the last 5 administrative logs."

**🤖 AI Agent:**
> I've listed the last 5 logs from the panel. They include recent site creations, database backups, and security configuration changes. Should I retrieve the full details for the most recent entry?


## ❓ FAQ

**Q: How do I find my Baota API Secret Key?**
Log in to your Baota Panel, go to [Panel Settings] -> [API Interface], enable the API toggle, and you will see your API Secret Key (api_sk).

**Q: Why do I need to whitelist my IP?**
Baota Panel requires all API callers to have their IP address explicitly whitelisted in the [API Interface] settings for security reasons. Without this, all requests will be blocked.

**Q: Can I check the system load in real-time?**
Yes! Use the `get_system_total` tool to retrieve current CPU, RAM, and system load averages, allowing your agent to monitor server performance instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baota-panel-api](https://vinkius.com/mcp/baota-panel-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baota Panel / 宝塔面板 API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baota-panel-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baota Panel / 宝塔面板 API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baota-panel-api": {
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
