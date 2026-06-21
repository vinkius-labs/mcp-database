# Checkmk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkmk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkmk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkmk-mcp)
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


## Installation & Usage

To install and use the **Checkmk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkmk](https://vinkius.com/mcp/checkmk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
