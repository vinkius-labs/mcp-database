# Plumbing Pipe Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/plumbing-pipe-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Deterministic water supply pipe sizing based on IPC and Hunter's Curve.

## Description
This MCP server provides precise water supply pipe sizing calculations following the International Plumbing Code (IPC). It uses Hunter's Curve to convert fixture units into required Gallons Per Minute (GPM) and accounts for simultaneous demand factors. Use `get_fixture_unit_reference` to find unit values, `calculate_demand_flow` to determine required flow, and `size_pipe_diameter` to select the optimal pipe size based on available pressure and pipe length.


## Available Tools (3)
- **calculate_demand_flow**: Calculates the expected Gallons Per Minute (GPM) required for a total fixture load
- **get_fixture_unit_reference**: Retrieves the fixture unit value for a specific plumbing fixture
- **size_pipe_diameter**: Determines the minimum required pipe diameter to meet demand while staying within pressure limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plumbing Pipe Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many fixture units is a standard toilet worth?"

**🤖 AI Agent:**
> A standard toilet is worth 3 fixture units.

---

**👤 You:**
> "What is the required GPM for 15 fixture units?"

**🤖 AI Agent:**
> The required demand flow rate for 15 fixture units is 18.5 GPM.

---

**👤 You:**
> "What pipe size do I need for 20 GPM, 50 PSI, and 40 feet of pipe?"

**🤖 AI Agent:**
> The minimum required pipe diameter is 1.0 inch.


## ❓ FAQ

**Q: How do I find the fixture unit value for a specific item?**
You can use the `get_fixture_unit_reference` tool to retrieve the standard IPC unit value for any recognized plumbing fixture.

**Q: What is Hunter's Curve used for in this tool?**
Hunter's Curve is used by the `calculate_demand_flow` tool to convert the total sum of fixture units into a realistic demand flow rate in GPM, accounting for simultaneous usage.

**Q: Can I specify a maximum pressure drop?**
Yes, when using `size_pipe_diameter`, you can provide an optional `targetPressureDropMax` to ensure the selected pipe size stays within your preferred pressure limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/plumbing-pipe-sizing](https://vinkius.com/ai-agent-connect/plumbing-pipe-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plumbing Pipe Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plumbing-pipe-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plumbing Pipe Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plumbing-pipe-sizing": {
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
