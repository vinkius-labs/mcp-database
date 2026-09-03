# Foundation Settlement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/foundation-settlement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate immediate, consolidation, and total soil settlement for foundation engineering.

## Description
This MCP server provides specialized geotechnical engineering tools to estimate ground movement. Use `get_immediate_settlement` to find instantaneous elastic deformation, `get_consolidation_settlement` for volume changes in cohesive soils like clay or silt, and `get_time_dependent_settlement` to track settlement progress over time. Finally, use `get_total_settlement` to combine these values for a complete settlement profile.


## Available Tools (4)
- **get_immediate_settlement**: Calculates the instantaneous elastic deformation of the soil under a given load
- **get_time_dependent_settlement**: Estimates the settlement occurring at a specific point in time due to the ongoing consolidation process
- **get_total_settlement**: Provides the combined settlement (Immediate + Consolidation) to determine the total expected movement
- **get_consolidation_settlement**: Calculates the volume change settlement resulting from pore water dissipation in cohesive soils


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foundation Settlement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the immediate settlement for a 5m x 5m foundation with a 1000kN load and a soil modulus of 20MPa."

**🤖 AI Agent:**
> The immediate settlement is 12.5 mm.

---

**👤 You:**
> "What is the consolidation settlement for a 10m thick clay layer under a 500kN load with a 5m x 5m foundation?"

**🤖 AI Agent:**
> The consolidation settlement for the clay layer is 25.0 mm.

---

**👤 You:**
> "If the total consolidation settlement is 30mm, what is the current settlement after 2 years with a consolidation coefficient of 0.1?"

**🤖 AI Agent:**
> The current settlement is 15.0 mm and the remaining settlement is 15.0 mm.


## ❓ FAQ

**Q: What is the difference between immediate and consolidation settlement?**
Immediate settlement is the instantaneous elastic response of the soil, while consolidation settlement is the time-dependent volume change caused by pore water dissipation in cohesive soils.

**Q: Can I calculate settlement for sand using the consolidation tool?**
No, consolidation settlement is specifically for cohesive soils like clay or silt. For sand, the consolidation settlement is treated as zero.

**Q: How do I get the total expected movement of a foundation?**
You can use the `get_total_settlement` tool, which sums the results from the immediate and consolidation settlement calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/foundation-settlement-calculator](https://vinkius.com/ai-agent-connect/foundation-settlement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foundation Settlement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foundation-settlement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foundation Settlement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foundation-settlement-calculator": {
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
