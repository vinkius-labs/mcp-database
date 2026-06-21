# Plumbing Fixture Units Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plumbing-fixture-units-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate DFU and WSFU loads and size plumbing pipe diameters according to IPC/UPCA standards.

## Description
This MCP server provides specialized tools for plumbing engineering calculations. Use `calculate_room_fixture_load` to determine the Drainage Fixture Units (DFU) and Water Supply Fixture Units (WSFU) for individual rooms based on fixture types and quantities. The `aggregate_building_load` tool allows you to sum these loads across multiple rooms to find the total building load. Finally, use `estimate_minimum_pipe_diameter` to determine the required minimum pipe diameter for horizontal branches or vertical stacks based on the calculated cumulative load.


## Available Tools (3)
- **aggregate_building_implements**: Calculates the total cumulative load for an entire building by summing multiple rooms
- **calculate_room_fixture_load**: Multiply these values by the provided quantity, then sum these products to reach the final totals for the room.

Calculates the combined drainage and water supply loads for a single room based on its fixtures
- **estimate_minimum_pipe_diameter**: The tool must find the lowest diameter where the specified load does not exceed the allowed threshold for that specific pipe type.

Determines the smallest required pipe diameter to safely handle a specific drainage or water supply load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plumbing Fixture Units Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the plumbing load for a bathroom with 1 toilet and 1 sink."

**🤖 AI Agent:**
> The total load for the bathroom is 4 DFU and 2 WSFU.

---

**👤 You:**
> "What is the minimum pipe diameter needed for a branch line with a load of 5 DFU?"

**🤖 AI Agent:**
> The minimum required diameter for a horizontal branch with 5 DFU is 2 inches.

---

**👤 You:**
> "Aggregate the loads from two rooms: Room A (3 DFU, 2 WSFU) and Room B (5 DFU, 4 WSFU)."

**🤖 AI Agent:**
> The total building load is 8 DFU and 6 WSFU.


## ❓ FAQ

**Q: How do I calculate the load for a single room?**
Use the `calculate_room_fixture_load` tool by providing a JSON array of fixtures, where each object includes the fixture type and its quantity.

**Q: Can I calculate the total load for an entire building?**
Yes, use the `aggregate_building_load` tool by passing in the results from your individual room calculations.

**Q: How does the pipe diameter estimation work?**
The `estimate_minimum_pipe_diameter` tool compares your current DFU or WSFU load against standard capacity limits for both horizontal branches and vertical stacks to find the smallest required diameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plumbing-fixture-units-calculator](https://vinkius.com/mcp/plumbing-fixture-units-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plumbing Fixture Units Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plumbing-fixture-units-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plumbing Fixture Units Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plumbing-fixture-units-calculator": {
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
