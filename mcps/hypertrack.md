# HyperTrack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hypertrack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hypertrack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hypertrack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage location tracking, trips, and geofences via HyperTrack API.

## Description
Empower your AI agents to manage your logistics and field operations with HyperTrack. This MCP server allows you to list tracked devices, monitor active trips, manage geofences, track field workers, and view order statuses directly through the HyperTrack API. Ideal for automating last-mile delivery and field service management.


## Available Tools
- **get_device**: Retrieves details for a specific device
- **get_geofence**: Retrieves details for a specific geofence
- **get_order**: Retrieves details for a specific order
- **get_trip**: Retrieves details for a specific trip
- **get_worker**: Retrieves details for a specific worker
- **list_devices**: Lists all registered devices
- **list_geofences**: Lists all geofences
- **list_orders**: Lists all orders
- **list_trips**: Lists all trips
- **list_workers**: Lists all workers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HyperTrack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all devices currently being tracked in HyperTrack."

**🤖 AI Agent:**
> I'll fetch the list of your active devices.

---

**👤 You:**
> "Show me the details for trip ID 'abc-123'."

**🤖 AI Agent:**
> I'll retrieve the detailed information for that trip.

---

**👤 You:**
> "Check for any active geofences in the system."

**🤖 AI Agent:**
> I'll look up the list of configured geofences for you.


## Installation & Usage

To install and use the **HyperTrack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hypertrack](https://vinkius.com/mcp/hypertrack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
