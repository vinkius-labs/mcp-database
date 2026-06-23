# HyperTrack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hypertrack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage location tracking, trips, and geofences via HyperTrack API.

## Description
Empower your AI agents to manage your logistics and field operations with HyperTrack. This MCP server allows you to list tracked devices, monitor active trips, manage geofences, track field workers, and view order statuses directly through the HyperTrack API. Ideal for automating last-mile delivery and field service management.


## Available Tools (10)
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


## ❓ FAQ

**Q: How do I get HyperTrack API credentials?**
You can find your Account ID and Secret Key in the HyperTrack dashboard under the Setup page.

**Q: Which version of the API is used?**
This MCP uses HyperTrack API v3, the latest version for location tracking and operations.

**Q: Can I track individual workers?**
Yes, the list_workers tool provides access to field worker metadata and their current tracking status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hypertrack](https://vinkius.com/mcp/hypertrack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HyperTrack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hypertrack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HyperTrack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hypertrack": {
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
