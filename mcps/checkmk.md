# Checkmk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkmk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage IT infrastructure monitoring via Checkmk — track hosts, monitor services, and activate changes directly from any AI agent.

## Description
Connect your **Checkmk** site to any AI agent and take full control of your IT infrastructure monitoring through natural conversation. Streamline how you manage complex server landscapes and service states.

### What you can do

- **Host Oversight** — List and retrieve detailed configuration and status for all monitored hosts natively
- **Service Intelligence** — Access real-time monitoring data for services across your entire infrastructure flawlessly
- **Configuration Control** — List folders, host groups, and service groups to understand your monitoring structure securely
- **Change Management** — Manually activate pending configuration changes directly within your workspace flawlessly
- **Live Diagnostics** — Retrieve plugin output and current states for specific services to troubleshoot issues in real-time
- **System Metadata** — Access core site information and organizational configurations directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkmk Username, Automation Secret, and Server URL (including site)
3. Start managing your infrastructure monitoring from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sysadmins & DevOps** — monitor server health and activate changes using natural language
- **IT Operations** — audit service states and host groups without opening the complex monitoring GUI
- **Support Teams** — quickly look up service failures and plugin outputs straight from their chat interface
- **Network Engineers** — verify connectivity and monitoring coverage for distributed host landscapes


## Available Tools
- **activate_checkmk_changes**: Activate pending configuration changes in Checkmk
- **get_host_details**: Get detailed information for a specific host
- **list_all_monitored_services**: List all services across all hosts
- **list_checkmk_folders**: List configuration folders
- **list_host_groups**: List configured host groups
- **list_checkmk_hosts**: List all monitored hosts
- **list_service_groups**: List configured service groups
- **list_host_services**: List all monitored services for a specific host


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkmk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my hosts in Checkmk."

**🤖 AI Agent:**
> Retrieving your hosts... I found 15 hosts including 'web-server-01', 'db-primary', and 'backup-node'. All appear to be Up except for 'backup-node' which is currently DOWN.

---

**👤 You:**
> "Show me the services for host 'web-server-01' that are not OK."

**🤖 AI Agent:**
> Checking services for web-server-01... I found 2 issues: 'CPU load' is WARNING (Load is 4.5) and 'Filesystem /var' is CRITICAL (98% full). Should I get more details?

---

**👤 You:**
> "Activate my pending changes in Checkmk."

**🤖 AI Agent:**
> Triggering activation of changes... The activation run has started. I will notify you once the monitoring core has been successfully updated with the new configuration.


## ❓ FAQ

**Q: Can I see failing services across all my hosts?**
Yes! Use the `list_all_monitored_services` tool. The agent will return a comprehensive list of services, and you can ask it to filter for those in CRITICAL or WARNING states.

**Q: How do I apply changes I made in WATO through the agent?**
Use the `activate_checkmk_changes` tool. Your agent will trigger the activation process in Checkmk, pushing all pending configurations to the monitoring core.

**Q: Where do I find my Checkmk Automation Secret?**
Log in to your Checkmk site, go to 'Setup' -> 'Users', and edit your automation user. You will see the 'Automation secret' field there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkmk](https://vinkius.com/mcp/checkmk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Checkmk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `checkmk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Checkmk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "checkmk": {
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
