# Jamf Pro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jamf-pro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jamf-pro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jamf-pro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage Apple devices, computers, and inventory via Jamf Pro API.

## Description
Empower your AI agents to manage your Apple ecosystem with Jamf Pro. This MCP server allows you to list mobile devices and computers, track inventory details, manage users and buildings, and view management scripts and packages directly through the Jamf Pro API. Ideal for automating IT operations and device management.


## Available Tools
- **get_computer**: Includes disk encryption status, installed apps, and user info. Use this for detailed Mac auditing.

Retrieves details for a specific computer
- **get_mobile_device**: Includes OS version, security status, and assigned user. Use this for deep investigation of a specific mobile asset.

Retrieves details for a specific mobile device
- **list_buildings**: Useful for auditing site-based device distribution.

Lists all configured buildings
- **list_categories**: Useful for navigating the management hierarchy.

Lists all management categories
- **list_computers**: Includes computer names, IDs, and serial numbers. Essential for auditing the Mac fleet.

Lists all managed computers
- **list_departments**: Use this to analyze device distribution by business unit.

Lists all configured departments
- **list_mobile_devices**: Returns device names, IDs, and models. Use this to audit the mobile device fleet.

Lists all managed mobile devices
- **list_packages**: pkg, .dmg) available in the Jamf Pro distribution points. Useful for auditing available software deployments.

Lists all software packages
- **list_scripts**: ) stored in Jamf Pro for remote execution. Useful for auditing custom automation assets.

Lists all management scripts
- **list_users**: Useful for identifying which users are associated with specific devices.

Lists all users in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jamf Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all computers managed in Jamf Pro."

**🤖 AI Agent:**
> I'll fetch the list of managed computers and their inventory details for you.

---

**👤 You:**
> "Show me details for mobile device ID '456'."

**🤖 AI Agent:**
> I'll retrieve the full inventory and management data for that mobile device.

---

**👤 You:**
> "List all management scripts configured in the system."

**🤖 AI Agent:**
> I'll look up the list of available management scripts in Jamf Pro.


## Installation & Usage

To install and use the **Jamf Pro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jamf-pro](https://vinkius.com/mcp/jamf-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
