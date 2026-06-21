# Kaseya MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kaseya)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kaseya-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kaseya-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage IT infrastructure, devices, and automation via Kaseya VSA 10.

## Description
Connect your **Kaseya VSA 10** instance to your AI agent for comprehensive IT management and remote monitoring. This MCP server enables your agent to interact with devices, scripts, and automation workflows across your managed environments.

### What you can do

- **Device Visibility** — List all managed agents and drill down into hardware/software details
- **Inventory Tracking** — Query organizations, groups, and assets to maintain a clear picture of your IT estate
- **Automation Management** — List and inspect scripts and automation workflows ready for deployment
- **Security Monitoring** — Access audit logs and active alarms to stay on top of system health and threats
- **Operational Insights** — Retrieve system information and health metadata for your VSA 10 instance

### How it works

1. Subscribe to this server
2. Enter your Kaseya Instance Name, Token ID, and Token Secret
3. Start managing your IT infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **IT Administrators** — Quickly check device status and trigger maintenance scripts via natural language
- **MSP Professionals** — Monitor multiple client organizations and alarms from a single interface
- **Security Teams** — Inspect audit logs and system health indicators effortlessly


## Available Tools
- **get_agent_details**: Get detailed information for a specific agent
- **list_agents**: Use this to check device availability and status.

List all managed agents (devices) in Kaseya
- **list_alarms**: List active system alarms
- **list_assets**: List managed assets
- **list_groups**: List all machine groups
- **list_audit_logs**: List recent audit logs
- **list_organizations**: List all organizations in Kaseya
- **list_scripts**: List agent scripts
- **get_system_info**: Get VSA 10 system information
- **list_workflows**: List automation workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kaseya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all agents that are currently offline in Kaseya."

**🤖 AI Agent:**
> I've scanned your managed devices. Out of 150 agents, 12 are currently offline, including 'Server-PROD-01' and 'WS-MARKETING-05'. Would you like more details on any of them?

---

**👤 You:**
> "Show me the recent audit logs for my VSA instance."

**🤖 AI Agent:**
> I've retrieved the latest audit logs. Recent actions include a policy update by 'Admin_User' and 3 successful script deployments to the 'Accounting' group.

---

**👤 You:**
> "List all machine groups in the organization."

**🤖 AI Agent:**
> I found 8 machine groups in your Kaseya instance, including 'Laptops', 'Production Servers', and 'Retail POS Systems'.


## Installation & Usage

To install and use the **Kaseya** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kaseya](https://vinkius.com/mcp/kaseya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
