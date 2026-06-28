# Column Sizing Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/column-sizing-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Preliminary sizing for reinforced concrete and steel columns based on vertical load accumulation.

## Description
The Column Sizing Estimator is a structural engineering utility designed for the early design phase of building projects. It allows engineers and architects to perform rapid pre-dimensioning of vertical supports by calculating cumulative axial loads and suggesting initial cross-sections for both reinforced concrete and steel profiles.

With this MCP server, AI agents can use `calculate_total_axial_load` to determine the total weight pressing down on a foundation based on floor count and tributary area. The toolset also includes `estimate_concrete_section` for determining square concrete dimensions, `estimate_steel_pattern` (via `estimate_steel_section`) for selecting standard HEB profiles, and `check_load_severity` to categorize projects into residential, commercial, or industrial tiers.


## Available Tools (4)
- **calculate_total_axial_load**: Calculates the total cumulative vertical force acting on the base of the column
- **estimate_concrete_section**: Suggests the minimum side dimensions for a square reinforced concrete column
- **check_load_severity**: Categorizes the total axial load into a recognizable engineering tier
- **estimate_steel_section**: Suggests a standard steel profile type for axial compression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Column Sizing Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total axial load for a 5-story building with an influence area of 50m² and a load of 10kN/m²."

**🤖 AI Agent:**
> The total accumulated axial load at the base is 2,500 kN.

---

**👤 You:**
> "What is the suggested concrete column size for a load of 1500 kN?"

**🤖 AI Agent:**
> The suggested dimension for the reinforced concrete column is 40 x 40 cm.

---

**👤 You:**
> "Suggest a steel profile for an axial load of 800 kN."

**🤖 AI Agent:**
> The recommended standard steel profile is HEB 160.


## ❓ FAQ

**Q: What is the purpose of this tool?**
It provides preliminary sizing for reinforced concrete and steel columns by calculating axial loads from building parameters.

**Q: Does this tool account for bending moments?**
No, this is a pre-dimensioning tool focused on axial loads only. It does not consider eccentricity or lateral forces.

**Q: Can I use it for industrial projects?**
Yes, the `check_load_severity` tool can identify high-load scenarios typical of industrial or infrastructure projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/column-sizing-estimator](https://vinkius.com/mcp/column-sizing-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Column Sizing Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `column-sizing-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Column Sizing Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "column-sizing-estimator": {
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
