# HPGR Circuit Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hpgr-circuit-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate HPGR roll dimensions, operating pressure, and throughput efficiency.

## Description
This MCP server provides technical engineering tools for High Pressure Grinding Rolls (HPGR) circuit design. It allows users to calculate essential equipment parameters such as roll dimensions using `get_roll_dimensions`, determine necessary pressing forces with `calculate_operating_pressure`, and evaluate material flow efficiency via `estimate_specific_throughput`. Additionally, it helps predict maintenance needs using `predict_roll_lifespan` based on ore abrasiveness and pressure.


## Available Tools (4)
- **calculate_operating_pressure**: Finds the necessary pressing force to achieve the desired product size
- **estimate_specific_throughput**: Calculates the efficiency of the material flow through the rolls
- **get_roll_dimensions**: Determines the physical size of the rolls required to meet a target throughput
- **predict_roll_lifespan**: Estimates how long the rolls will last before requiring maintenance based on wear


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HPGR Circuit Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What roll dimensions do I need for a throughput of 500 tph and an ore hardness of 15?"

**🤖 AI Agent:**
> The required roll diameter is 2.5 meters and the roll width is 1.8 meters.

---

**👤 You:**
> "Calculate the operating pressure for an ore with hardness 12, target size 5mm, and 5% moisture."

**🤖 AI Agent:**
> The specific pressure required is 3.2 N/mm² with a total force of 450 kN.

---

**👤 You:**
> "Estimate the lifespan for an abrasive ore (index 8) at 3 N/mm² pressure and 400 tph throughput."

**🤖 AI Agent:**
> The estimated operating life is 4,500 hours with a wear rate of 0.02 mm per hour.


## ❓ FAQ

**Q: How do I calculate the required roll size?**
Use the `get_roll_dimensions` tool by providing the target throughput and the ore hardness.

**Q: Can I predict how long the rolls will last?**
Yes, the `predict_roll_lifespan` tool estimates operating hours based on ore abrasiveness and operating pressure.

**Q: What inputs are needed for pressure calculations?**
You need to provide the ore hardness, the target product size, and the moisture content to `calculate_operating_pressure`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hpgr-circuit-design-tool](https://vinkius.com/en/ai-agent-connect/hpgr-circuit-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HPGR Circuit Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hpgr-circuit-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HPGR Circuit Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hpgr-circuit-design-tool": {
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
