# Gridscale (IaaS & PaaS Cloud Hosting API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Gridscale cloud infrastructure — provision servers, monitor metrics, and control PaaS services directly from any AI agent.

## Description
Connect your **Gridscale** account to any AI agent to manage your cloud infrastructure through natural language. This MCP server provides comprehensive access to Gridscale's IaaS and PaaS capabilities.

### What you can do

- **Server Lifecycle** — List, create, and manage the power state (on/off/shutdown) of your cloud servers.
- **Managed Services (PaaS)** — Access and list your managed databases, Redis instances, and other platform services.
- **Networking & Security** — Manage IP addresses, private networks, and firewall rules directly.
- **Storage & Media** — List storage volumes, ISO images, and templates for rapid deployment.
- **Performance Monitoring** — Retrieve real-time metrics for CPU usage and storage IOPS to ensure your infrastructure is healthy.

### How it works

1. Subscribe to this server
2. Enter your Gridscale User ID and API Token
3. Start managing your cloud resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate infrastructure audits and quick server restarts without leaving the terminal or chat.
- **Developers** — Provision test environments and check database service statuses during the coding process.
- **System Administrators** — Monitor resource metrics and manage network configurations through simple conversation.


## Available Tools (17)
- **create_server**: Create a new cloud server
- **get_server_metrics**: Get metrics for a specific server
- **get_server_power**: Get the power status of a specific server
- **link_ip_to_server**: Link an IP address to a server
- **link_storage_to_server**: Server usually needs to be powered off.

Link a storage volume to a server
- **list_deleted**: Useful for historical tracking.

List deleted objects
- **list_firewalls**: List all firewalls
- **list_ips**: List all IP addresses
- **list_iso_images**: List all ISO images
- **list_locations**: g., fra for Frankfurt) to use when creating resources.

List available datacenters/locations
- **list_networks**: List all networks
- **list_paas**: List all Platform Services (PaaS)
- **list_servers**: List all servers in your Gridscale account
- **list_storages**: List all storage volumes
- **list_templates**: List all templates
- **set_server_power**: Set the power status of a server
- **shutdown_server**: Perform an ACPI shutdown on a server


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gridscale (IaaS & PaaS Cloud Hosting API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active servers in Gridscale."

**🤖 AI Agent:**
> I've retrieved your server list. You have 3 servers: 'Production-Web' (Online), 'Staging-App' (Online), and 'Legacy-DB' (Offline). Would you like to see the metrics for any of them?

---

**👤 You:**
> "Create a new server named 'Dev-Node' with 2 cores and 4GB RAM."

**🤖 AI Agent:**
> I am initiating the creation of 'Dev-Node' with 2 CPU cores and 4GB RAM. I'll need a location UUID to proceed—should I list the available locations for you?

---

**👤 You:**
> "Show me the performance metrics for server uuid-789-xyz."

**🤖 AI Agent:**
> Fetching metrics for server uuid-789-xyz... In the last 15 minutes, CPU usage was stable at 15% and storage IOPS averaged 320. The server is performing within normal parameters.


## ❓ FAQ

**Q: Can I check the power status of a specific server using its UUID?**
Yes! Use the `get_server_power` tool with the server's UUID. The agent will return whether the server is currently powered on or off.

**Q: How do I monitor the performance of my cloud servers?**
You can use the `get_server_metrics` tool. It retrieves data in 15-minute intervals for core usage and storage IOPS, allowing your AI to analyze resource consumption.

**Q: Does this integration support managed databases like MySQL or PostgreSQL?**
Yes, you can list all managed Platform Services (PaaS) including MySQL, PostgreSQL, and Redis using the `list_paas` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api](https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gridscale (IaaS & PaaS Cloud Hosting API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gridscale-iaas-paas-cloud-hosting-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gridscale (IaaS & PaaS Cloud Hosting API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gridscale-iaas-paas-cloud-hosting-api": {
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
