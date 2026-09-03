# Pile Load Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pile-load-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate pile axial capacity, allowable load, and settlement.

## Description
This MCP server provides specialized geotechnical engineering tools to determine the axial capacity of piles. It calculates the ultimate capacity by summing skin friction and end bearing based on soil layers and SPT values. Users can also determine the safe working load using `calculate_allowable_capacity` and predict vertical displacement with `estimate_settlement`. The server accounts for pile geometry via `get_pile_geometry_properties`, groundwater depth, and installation methods like driven or bored piles.


## Available Tools (4)
- **calculate_allowable_capacity**: Calculate the safe working load for the pile
- **get_pile_geometry_properties**: Retrieve geometric constants (area, perimeter) based on pile type
- **estimate_settlement**: Predict the vertical displacement of the pile under a given load
- **calculate_ultimate_capacity**: Calculate the total theoretical axial capacity of a pile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pile Load Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ultimate capacity of a cylindrical pile with a 500mm diameter and 15m length in these soil layers: [{"depth": 10, "spt": 20, "type": "sand"}, {"depth": 5, "spt": 35, "type": "clay"}] with groundwater at 5m, installed as driven?"

**🤖 AI Agent:**
> The ultimate capacity for the specified cylindrical pile is 2450.5 kN, consisting of 1850.2 kN skin friction and 600.3 kN end bearing.

---

**👤 You:**
> "Calculate the allowable capacity for a pile with an ultimate capacity of 3000 kN and a factor of safety of 2.5."

**🤖 AI Agent:**
> The allowable capacity is 1200.0 kN.

---

**👤 You:**
> "Estimate the settlement for a 400mm diameter pile, 10m long, under a 500kN load with the provided soil profile and groundwater at 2m."

**🤖 AI Agent:**
> The estimated total settlement is 12.4 mm, comprising 8.2 mm of elastic settlement and 4.2 mm of consolidation settlement.


## ❓ FAQ

**Q: How is the ultimate capacity calculated?**
The `calculate_ultimate_capacity` tool calculates the total resistance by summing the skin friction across all soil layers and the end bearing at the pile tip, adjusted for groundwater depth.

**Q: Can I calculate the safe working load?**
Yes, you can use `calculate_allowable_capacity` to find the safe working load by applying a factor of safety to the ultimate capacity.

**Q: Does the tool account for different pile shapes?**
Yes, the server supports cylindrical and square piles. You can use `get_pile_geometry_properties` to retrieve specific area and perimeter values for these shapes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pile-load-capacity-calculator](https://vinkius.com/ai-agent-connect/pile-load-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pile Load Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pile-load-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pile Load Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pile-load-capacity-calculator": {
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
