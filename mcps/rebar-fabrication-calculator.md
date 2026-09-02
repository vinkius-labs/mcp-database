# Rebar Fabrication Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rebar-fabrication-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise rebar cutting lengths, bend deductions, and hook requirements.

## Description
This MCP server provides precision tools for rebar fabrication. It accounts for material stretch during bending by calculating bend deductions and bend allowances. Use `calculate_total_cut_length` to determine the exact raw stock length needed, or use `get_bend_deduction` and `get_hook_length` for individual component calculations. It ensures structural accuracy for reinforcement steel.


## Available Tools (4)
- **calculate_total_cut_length**: Calculates the final length of the bar to be cut from the raw stock
- **get_bend_allowance**: Determines the centerline arc length for a specific bend
- **get_bend_deduction**: Calculates the amount of length to subtract from the total segments to account for material stretch
- **get_hook_length**: Calculates the additional steel required to create a specific end hook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebar Fabrication Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cut length for a 12mm rebar with a 90-degree bend, 30mm radius, and a 90_DEGREE hook, where the straight segments sum to 2 meters?"

**🤖 AI Agent:**
> The total cut length required is 2054.2 mm.

---

**👤 You:**
> "Calculate the bend deduction for a 16mm bar with a 45-degree bend and 40mm radius."

**🤖 AI Agent:**
> The bend deduction is 10.5 mm.

---

**👤 You:**
> "How much extra length is needed for a 135_DEGREE hook on a 10mm rebar?"

**🤖 AI Agent:**
> The required hook length is 45.0 mm.


## ❓ FAQ

**Q: How does this tool account for steel stretching?**
The tool uses `get_bend_deduction` to calculate the length lost due to material stretch during the bending process, ensuring the final dimensions are correct.

**Q: What hook types are supported?**
It supports standard and seismic hooks, such as 90_DEGREE and 135_DEGREE, via the `get_hook_length` tool.

**Q: Can I calculate the total length in one step?**
Yes, use the `calculate_total_cut_length` tool to get the total cut length, bend deduction, hook length, and allowance in a single response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rebar-fabrication-calculator](https://vinkius.com/ai-agent-connect/rebar-fabrication-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rebar Fabrication Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rebar-fabrication-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rebar Fabrication Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rebar-fabrication-calculator": {
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
