# Kandji MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kandji)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kandji-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kandji-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Manage Apple devices, blueprints, and security via Kandji MDM API.

## Description
Empower your AI agents with Kandji's modern Apple MDM platform. This MCP server allows you to list and retrieve device details, manage blueprints and custom apps, track administrative activity, and view system security parameters directly through the Kandji API. Ideal for automating IT operations and fleet security for macOS and iOS.


## Available Tools
- **get_device**: Essential for deep-dive auditing of a specific asset.

Retrieves details for a specific device
- **get_organization**: Use to verify account identity.

Retrieves details about your Kandji organization
- **list_activity**: Essential for auditing system changes and recent management history.

Lists recent management activity
- **list_auto_apps**: Essential for auditing standard software libraries.

Lists all Kandji Auto Apps
- **list_blueprints**: Useful for understanding how devices are categorized and configured.

Lists all device blueprints
- **list_commands**: g., Lock, Wipe, Restart) sent to managed devices. Useful for auditing remote actions.

Lists recent MDM commands sent to devices
- **list_custom_apps**: Useful for auditing non-store software deployments.

Lists all custom applications
- **list_devices**: Returns device names, IDs, and OS versions. Use this as the main tool for auditing the device fleet.

Lists all managed Apple devices in Kandji
- **list_parameters**: Useful for auditing available security controls.

Lists all library parameters (policies)
- **list_users**: Useful for identifying device owners and primary users.

Lists all users associated with devices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kandji** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all managed Mac computers in Kandji."

**🤖 AI Agent:**
> I'll fetch the list of all Apple devices currently enrolled in your Kandji account.

---

**👤 You:**
> "Show me the details for device ID 'abc-123'."

**🤖 AI Agent:**
> I'll retrieve the full inventory and security metadata for that specific Apple device.

---

**👤 You:**
> "Check recent administrative activity in Kandji."

**🤖 AI Agent:**
> I'll look up the log of recent management actions and system events in your Kandji account.


## Installation & Usage

To install and use the **Kandji** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kandji](https://vinkius.com/mcp/kandji)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
