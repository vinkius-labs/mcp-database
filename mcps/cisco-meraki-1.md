# Cisco Meraki MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cisco-meraki-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cisco-meraki-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cisco-meraki-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Cloud-managed IT via Cisco Meraki — track networks, devices, and client connectivity.

## Description
Connect your **Cisco Meraki** dashboard to any AI agent and take full control of your cloud-managed IT infrastructure through natural conversation.

### What you can do

- **Organization Oversight** — List all organizations and fetch detailed metadata for specific entities
- **Network Orchestration** — Enumerate networks within an organization and retrieve detailed configurations
- **Hardware Inventory** — List all devices (APs, switches, security appliances) and monitor real-time statuses
- **Client Monitoring** — Track connected clients, their signal strength, and connectivity metrics securely
- **Wireless Management** — List configured SSIDs and inspect specific wireless settings across your networks

### How it works

1. Subscribe to this server
2. Enter your Cisco Meraki API Key
3. Start managing your IT infrastructure from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_device**: Get details for a specific device
- **get_device_statuses**: Get statuses for all devices in an organization
- **get_organization**: Get details for a specific organization
- **get_appliance_settings**: Get appliance settings for a network
- **list_clients**: ) for a specific network.

List clients on a network
- **list_devices**: List devices within a network
- **list_networks**: List networks within an organization
- **list_organizations**: List all organizations
- **list_wireless_ssids**: List SSIDs for a wireless network
- **search_organizations**: Search organizations by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cisco Meraki** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations I have access to in Meraki."

**🤖 AI Agent:**
> Retrieving organizations... I found your authorized entities, including 'Global Enterprise' and 'Regional Branch'.

---

**👤 You:**
> "Show status for all devices in network ID 'N_12345'."

**🤖 AI Agent:**
> Checking device statuses... Network 'N_12345' has 10 online devices and 1 alerting access point.

---

**👤 You:**
> "Search for connected clients in the 'San Francisco Office' network."

**🤖 AI Agent:**
> Querying connected clients... I identified 50 active clients, including 30 mobile devices and 20 laptops.


## Installation & Usage

To install and use the **Cisco Meraki** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cisco-meraki-1](https://vinkius.com/mcp/cisco-meraki-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
