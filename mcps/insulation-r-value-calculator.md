# Insulation R-Value Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/insulation-r-value-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate minimum insulation R-values, required thickness, and estimated costs based on IECC climate zones.

## Description
This MCP server provides a specialized calculation engine for building insulation requirements. By using the `lookup_zone_requirements` tool, you can retrieve mandatory R-values for walls, ceilings, floors, and basements based on specific IECC climate zones (1-8). Additionally, use `calculate_material_thickness` to determine how many inches of batt, spray foam, or rigid insulation are needed to meet a target R-value, and `estimate_material_cost` to project the total cost for your insulation project based on area and material thickness.


## Available Tools (3)
- **calculate_material_thickness**: Calculates required insulation thickness
- **estimate_material_cost**: Estimates insulation cost
- **lookup_zone_requirements**: Retrieves minimum R-values for a specific IECC climate zone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insulation R-Value Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the minimum R-value requirements for climate zone 5?"

**🤖 AI Agent:**
> In IECC Climate Zone 5, the minimum required R-values are: Walls: R-13, Ceilings: R-38, Floors: R-10, and Basements: R-7.

---

**👤 You:**
> "How thick does spray foam need to be to achieve an R-value of 25?"

**🤖 AI Agent:**
> To achieve a target R-value of 25 using spray foam, you will need a thickness of approximately 3.13 inches.

---

**👤 You:**
> "Estimate the cost for insulating 1000 sq ft with 5 inches of rigid insulation."

**🤖 AI Agent:**
> The estimated cost for 1,000 square feet of rigid insulation at a thickness of 5 inches is $1,250.00 (approximately $1.25 per sq ft).


## ❓ FAQ

**Q: How do I find the required R-value for my area?**
Use the `lookup_zone_requirements` tool by providing your specific IECC climate zone number (between 1 and 8).

**Q: Can I estimate the cost of my insulation project?**
Yes, use the `estimate_material_cost` tool with your area in square feet, material type, and required thickness to get a projection.

**Q: What insulation materials are supported?**
The tool supports 'batt', 'spray_foam', and 'rigid' insulation types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/insulation-r-value-calculator](https://vinkius.com/mcp/insulation-r-value-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insulation R-Value Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insulation-r-value-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insulation R-Value Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insulation-r-value-calculator": {
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
