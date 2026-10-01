# Material Inventory Gap Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/material-inventory-gap-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Analyze material shortages, excesses, and required purchase quantities against project needs.

## Description
This MCP server provides tools to reconcile project requirements with physical inventory. It calculates the Available-to-Promise (ATP) quantity by accounting for reserved stock and handles unit conversions. Use `calculate_material_gap` to identify shortages and determine the exact purchase quantity needed based on package sizes, or `get_material_availability` to check current stock levels and commitments.


## Available Tools (4)
- **calculate_material_gap**: Determines if a specific material is sufficient for a project or if more must be bought
- **list_project_requirements**: Retrieves the full list of materials and quantities needed for a specific project
- **get_conversion_factor**: Determines the multiplier needed to convert between different units for a specific material
- **get_material_availability**: Provides a snapshot of a material's status, including total stock and committed stock


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Material Inventory Gap Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if we have enough cement for project PROJ-101. We need 50 bags."

**🤖 AI Agent:**
> There is a shortage of 12 bags for project PROJ-101. You need to purchase 12 more bags to meet the requirement.

---

**👤 You:**
> "What is the current availability for material MAT-99?"

**🤖 AI Agent:**
> Material MAT-99 has a total inventory of 500 units, with 100 units currently reserved. The available-to-promise quantity is 400 units.

---

**👤 You:**
> "List all materials required for project REQ-500."

**🤖 AI Agent:**
> Project REQ-500 requires: 50 units of Steel (MAT-01), 20 units of Concrete (MAT-05), and 10 units of Gravel (MAT-09).


## ❓ FAQ

**Q: How does the tool calculate shortages?**
The `calculate_material_gap` tool subtracts all reserved stock from the total inventory to find the Available-to-Promise quantity. If the project requirement is higher than this amount, a shortage is reported.

**Q: Can I convert units between different materials?**
Yes, you can use `get_conversion_factor` to find the multiplier needed to convert between different units for a specific material.

**Q: How are purchase quantities determined?**
Purchase quantities are calculated by taking the required shortage and rounding it up to the nearest increment defined by the material's package size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/material-inventory-gap-analysis](https://vinkius.com/en/ai-agent-connect/material-inventory-gap-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Material Inventory Gap Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `material-inventory-gap-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Material Inventory Gap Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "material-inventory-gap-analysis": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
