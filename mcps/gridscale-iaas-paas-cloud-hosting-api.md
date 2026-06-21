# Gridscale (IaaS & PaaS Cloud Hosting API) MCP Server

Manage your Gridscale cloud infrastructure — provision servers, monitor metrics, and control PaaS services directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api)

## Overview
**Category:** developer-tools
**Tools Count:** 17

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


## Available Tools
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


## Installation & Usage

To install and use the **Gridscale (IaaS & PaaS Cloud Hosting API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api](https://vinkius.com/mcp/gridscale-iaas-paas-cloud-hosting-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
