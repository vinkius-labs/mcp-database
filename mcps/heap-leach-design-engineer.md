# Heap Leach Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/heap-leach-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Professional engineering tool for designing gold and copper heap leach pads.

## Description
This MCP server provides specialized hydrometallurgical engineering tools for designing heap leach pads used in gold and copper extraction. It allows engineers to calculate pad footprints, optimize irrigation rates to prevent flooding, validate stack stability based on ore density and angle of repose, and estimate total leach cycle durations. Use `calculate_pad_footprint_tool` to determine surface area, `optimize_irrigation_flow_tool` for fluid dynamics, `validate_stack_stability_tool` for structural safety, and `estimate_leach_duration_tool` for process timing.


## Available Tools (4)
- **optimize_irrigation_flow_tool**: Calculates the necessary irrigation rate to maintain optimal moisture without surface flooding
- **calculate_pad_footprint_tool**: Determines the required surface area of the leach pad based on total ore volume and preferred stack height
- **estimate_leach_duration_tool**: Predicts how long the leach cycle will last given the ore volume and irrigation capacity
- **validate_stack_stability_tool**: Checks if the proposed stack height is safe based on the ore's physical properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heap Leach Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pad area needed for 500,000 cubic meters of ore with a target stack height of 5 meters."

**🤖 AI Agent:**
> The required pad area is 100,000 square meters.

---

**👤 You:**
> "Is a 10-meter stack stable for ore with a density of 2.5 and an angle of repose of 35 degrees?"

**🤖 AI Agent:**
> Yes, the stack is stable with a safety factor of 1.4.

---

**👤 You:**
> "What is the irrigation rate for a 50,000 square meter pad with an ore permeability of 0.5?"

**🤖 AI Agent:**
> The optimal irrigation rate is 250 cubic meters per hour, with a Low risk level for flooding.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate pad area, stack stability, irrigation rates, and the total duration of the leach cycle using specialized engineering models.

**Q: How do I ensure my stack is stable?**
Use the `validate_stack_stability_tool` by providing the proposed height, ore density, and the angle of repose to check the safety factor.

**Q: Can I optimize irrigation for different ore types?**
Yes, the `optimize_irrigation_flow_tool` uses ore permeability to calculate the ideal irrigation rate and assess flooding risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/heap-leach-design-engineer](https://vinkius.com/ai-agent-connect/heap-leach-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heap Leach Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heap-leach-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heap Leach Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heap-leach-design-engineer": {
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
