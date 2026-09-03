# Excavation Volume Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/excavation-volume-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise earthwork volumes, including cut, loose, and backfill requirements.

## Description
This MCP server provides professional engineering tools for earthwork calculations. It allows AI agents to determine the exact volume of soil to be removed using `get_cut_volume`, calculate the expanded volume for transport with `get_loose_volume`, and determine necessary soil amounts for filling voids via `get_backfill_requirement`. It also includes `get_soil_properties_lookup` to retrieve standard swell, compaction, and shrinkage factors for various soil types like sand, clay, or gravel.


## Available Tools (4)
- **get_backfill_requirement**: Calculates the volume of soil needed to fill a specific space, accounting for how the soil will compress
- **get_cut_volume**: Calculates the primary volume of soil to be removed from the ground based on excavation geometry
- **get_loose_volume**: Determines the volume the soil will occupy during transport and stockpiling
- **get_soil_properties_lookup**: Provides standard physical constants for different soil types to be used in volume calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Excavation Volume Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cut volume for an excavation 10m long, 5m wide, 3m deep, with a 45 degree slope angle."

**🤖 AI Agent:**
> The total cut volume for the excavation is 210.0 m³.

---

**👤 You:**
> "If I have 100 m³ of bank volume and the swell factor for sand is 1.2, what is the loose volume?"

**🤖 AI Agent:**
> The loose volume for 100 m³ of sand with a 1.2 swell factor is 120.0 m³.

---

**👤 You:**
> "How much bank volume is needed to fill a 50 m³ void if the compaction factor is 0.9?"

**🤖 AI Agent:**
> To fill a 50 m³ void with a compaction factor of 0.9, you will need 55.56 m³ of bank volume.


## ❓ FAQ

**Q: How does the tool account for soil expansion?**
The tool uses the `get_loose_volume` function which applies a swell factor to the bank volume to determine the total space the soil will occupy once excavated.

**Q: Can I get specific soil constants?**
Yes, you can use `get_soil_properties_lookup` to retrieve standard swell, compaction, and shrinkage factors for common soil types.

**Q: What is the difference between bank and loose volume?**
Bank volume is the soil in its natural state, while loose volume is the expanded volume after excavation, calculated using the swell factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/excavation-volume-calculator](https://vinkius.com/ai-agent-connect/excavation-volume-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Excavation Volume Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `excavation-volume-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Excavation Volume Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "excavation-volume-calculator": {
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
