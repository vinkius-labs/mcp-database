# HetrixTools MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hetrixtools)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Automate uptime monitoring and blacklist checks via HetrixTools — monitor servers, websites, and IP reputation directly from any AI agent.

## Description
Connect your **HetrixTools** account to any AI agent and take full control of your infrastructure monitoring and IP reputation management through natural conversation.

### What you can do

- **Uptime Oversight** — List all uptime monitors, check status, and retrieve detailed availability reports for your websites and services.
- **Blacklist Monitoring** — List and manage monitors for IP addresses and domains across 90+ global blacklists.
- **On-Demand Checks** — Perform real-time blacklist scans for any IPv4 address or domain directly from the chat.
- **Maintenance Control** — Quickly toggle maintenance modes for your monitors to avoid false alerts during updates.
- **Resource Tracking** — Monitor your account's API and monitor usage to stay within your plan limits.
- **Team Alerts** — Access and manage your contact lists to ensure the right people are notified of outages.

### How it works

1. Subscribe to this server
2. Enter your HetrixTools API Token (found in Account Settings > API)
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

No more manual checking of monitoring dashboards. Your AI assistant acts as a dedicated Infrastructure Monitor or System Administrator.

### Who is this for?

- **DevOps Engineers** — instantly check server health and toggle maintenance modes without leaving the terminal.
- **System Administrators** — automate the auditing of IP reputation and domain blacklist status.
- **Website Owners** — monitor website uptime and receive instant reports on any service interruptions.


## Available Tools (11)
- **add_uptime_monitor**: Pass the configuration as a JSON string in "body_json" (requires type, target, label, and contact ID).

Create a new uptime monitor
- **check_domain_blacklist**: Useful for identifying mail delivery issues.

Perform an on-demand blacklist check for a domain
- **check_ip_blacklist**: Note: results may take a few minutes to process.

Perform an on-demand blacklist check for an IPv4 address
- **delete_uptime_monitor**: Remove an uptime monitor
- **get_account_usage**: Retrieve current API and resource usage statistics
- **list_blacklist_monitors**: List all IP and domain blacklist monitors
- **list_bulk_reports**: List all generated bulk reports
- **list_contact_lists**: List notification contact lists
- **list_uptime_monitors**: Use this to check the current health of your infrastructure.

List all uptime monitors
- **list_uptime_reports**: Retrieve detailed uptime reports for a monitor
- **set_maintenance_mode**: Modes: 1 (Normal), 2 (Maint. with notifications), 3 (Maint. without notifications).

Toggle maintenance mode for an uptime monitor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HetrixTools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my uptime monitors and their current status."

**🤖 AI Agent:**
> I've retrieved your monitors. You have 5 active checks: 'Primary Website' (Up), 'API Endpoint' (Up), 'DB Server' (Up), 'Mail Gateway' (Up), and 'Staging Site' (Down - since 5 mins ago). Would you like to see the error log for the Staging Site?

---

**👤 You:**
> "Check if the IP address 1.2.3.4 is blacklisted."

**🤖 AI Agent:**
> Blacklist check initiated for 1.2.3.4. I've scanned 94 global blacklists. The IP is currently CLEAN (0/94 listings). Would you like to add this IP to your permanent blacklist monitors?

---

**👤 You:**
> "Put monitor ID 'm123' into maintenance mode without notifications."

**🤖 AI Agent:**
> Maintenance mode updated! Monitor m123 is now in mode 3 (Maintenance without notifications). You can perform your updates without triggering any alerts. Should I list your other monitors?


## ❓ FAQ

**Q: How do I find my HetrixTools API Token?**
Log in to your HetrixTools account, navigate to **Account Settings**, and click on the **API** tab. You will be able to generate and copy your unique API Token from there.

**Q: Can I perform on-demand blacklist checks?**
Yes! Use the `check_ip_blacklist` or `check_domain_blacklist` tools. These trigger real-time scans across 90+ blacklists. Note that these requests can take a few minutes to complete.

**Q: What are the maintenance modes for monitors?**
The integration supports three modes: 1 (Normal), 2 (Maintenance with notifications enabled), and 3 (Maintenance without notifications). Use `set_maintenance_mode` to toggle these.

**Q: Is the integration secure for monitoring data?**
Absolutely. The integration uses industry-standard Bearer tokens (v3) or secure URL tokens over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hetrixtools](https://vinkius.com/mcp/hetrixtools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HetrixTools** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hetrixtools` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HetrixTools** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hetrixtools": {
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
