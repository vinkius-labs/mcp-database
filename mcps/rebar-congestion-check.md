# Rebar Congestion Check MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rebar-congestion-check)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Analyzes reinforcement density and concrete placement feasibility.

## Description
This MCP server provides structural engineering tools to evaluate reinforcement density in concrete sections. It allows AI agents to verify if rebar spacing is sufficient for aggregate passage, ensure mechanical vibrators can access the cage, and calculate a congestion score to prevent honeycombing. Use `calculate_clear_spacing` to find physical gaps, `check_aggregate_passage` to verify aggregate flow, `evaluate_vibration_access` for tool clearance, and `get_congestion_score` for a density assessment.


## Available Tools (4)
- **evaluate_vibration_access**: Checks if there is enough room for a concrete vibration tool to enter the cage
- **calculate_clear_spacing**: Determines the actual physical gap between rebar elements
- **check_aggregate_passage**: Verifies if the specified concrete aggregate can pass through the rebar cage
- **get_congestion_score**: Provides a high-level assessment of the reinforcement density


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebar Congestion Check** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if 20mm aggregate can pass through a cage with 16mm bars in a 300x300mm section with 40mm cover and 2 layers."

**🤖 AI Agent:**
> The aggregate can pass through the reinforcement cage.

---

**👤 You:**
> "What is the congestion score for 25mm bars in a 500x500mm section with 50mm cover and 3 layers?"

**🤖 AI Agent:**
> The congestion score is 15, which is considered Low risk.

---

**👤 You:**
> "Will a 40mm vibrator needle fit in a section with 12mm bars and 30mm clear cover?"

**🤖 AI Agent:**
> No, the vibrator needle cannot access the target areas.


## ❓ FAQ

**Q: How do I check if my aggregate will fit between the bars?**
You can use the `check_aggregate_passage` tool by providing the bar sizes, section dimensions, and the maximum aggregate diameter.

**Q: Can this tool help prevent concrete honeycombing?**
Yes, by using `get_congestion_score` and `evaluate_vibration_access`, you can identify if the reinforcement is too crowded for proper concrete consolidation.

**Q: What information is needed for the spacing calculation?**
To use `calculate_clear_spacing`, you need the array of bar diameters, the number of layers, the section width and height, and the clear cover.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rebar-congestion-check](https://vinkius.com/ai-agent-connect/rebar-congestion-check)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebar Congestion Check** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rebar-congestion-check` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebar Congestion Check** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebar-congestion-check": {
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
