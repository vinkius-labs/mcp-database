# Cisco Meraki MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cisco-meraki)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cisco-meraki-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cisco-meraki-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage cloud-managed networking via Cisco Meraki — track devices, monitor clients, and audit network health directly from any AI agent.

## Description
Connect your **Cisco Meraki** dashboard to any AI agent and take full control of your cloud-managed IT infrastructure through natural conversation. Streamline how you monitor wireless, switching, and security appliances.

### What you can do

- **Organization Oversight** — List and retrieve details for all organizations and networks under your administration natively
- **Device Intelligence** — Access real-time status and detailed metadata for APs, switches, and security appliances flawlessly
- **Client Monitoring** — List and track connected clients across your networks to understand usage securely
- **Inventory Logistics** — Audit your entire organization's device inventory and serial numbers flawlessly
- **Admin Tracking** — List and review organization administrators and their access levels securely
- **Network Summaries** — Retrieve comprehensive health summaries and configuration details directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cisco Meraki Dashboard API Key (obtained from your profile settings)
3. Start managing your cloud networks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Network Administrators** — monitor device uptime and client connectivity using natural language
- **IT Managers** — audit network health and device inventory without opening the dashboard
- **Support Teams** — quickly look up client details and device statuses straight from their chat interface
- **Security Engineers** — verify firewall status and administrator access levels


## Available Tools
- **get_device_details**: Get detailed information for a specific device by serial
- **get_network_summary**: Get summary details for a specific network
- **list_organization_admins**: List all administrators for an organization
- **list_network_clients**: List all connected clients in a network
- **list_network_devices**: List all physical devices (APs, Switches, Firewalls) in a network
- **list_organization_inventory**: List all devices in the organization inventory
- **list_organization_networks**: List all networks within an organization
- **list_meraki_organizations**: List all organizations the API key has access to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cisco Meraki** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Meraki organizations."

**🤖 AI Agent:**
> Retrieving your organizations... I found 2: 'Acme Corp' (ID: 123456) and 'Global Distribution' (ID: 789012). Which one would you like to explore?

---

**👤 You:**
> "Show me the status of devices in the 'London Office' network."

**🤖 AI Agent:**
> Checking 'London Office' devices... You have 1 MR42 (Online), 1 MS120 (Online), and 1 MX64 Security Appliance (Online). Everything looks healthy.

---

**👤 You:**
> "How many clients are currently connected to my wireless network?"

**🤖 AI Agent:**
> Retrieving client count... There are currently 45 clients connected across your active networks. 30 are on the 'Main-Staff' SSID and 15 are on 'Guest-WiFi'.


## Installation & Usage

To install and use the **Cisco Meraki** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cisco-meraki](https://vinkius.com/mcp/cisco-meraki)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
