# Material Selection Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/material-selection-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Identify, rank, and compare engineering materials based on environmental conditions and performance requirements.

## Description
This MCP server provides a decision-support system for engineering material selection using Ashby-style methodology. It allows AI agents to identify suitable materials by evaluating operating conditions and mandatory constraints. Users can use `find_suitable_materials` to filter candidates, `rank_materials` to optimize for specific performance indices like stiffness-to-weight, `compare_material_properties` for side-by-side data analysis, and `evaluate_manufacturability_and_cost` to assess production feasibility. It is designed to work with Cursor, VS Code, Claude Desktop, and Windsurf via Vinkius Edge.


## Available Tools (4)
- **compare_material_properties**: Provides a side-by-side comparison of specific properties between two or more materials
- **evaluate_manufacturability_and_cost**: Assesses the economic and production feasibility of the selected materials
- **find_suitable_materials**: Identifies a list of materials that satisfy all mandatory constraints and operating conditions
- **rank_materials**: Orders the suitable materials based on a specific performance goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Material Selection Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find materials that can withstand 500°C and have a minimum yield strength of 200 MPa."

**🤖 AI Agent:**
> The following materials meet your thermal and strength requirements: Titanium Alloy Ti-6Al-4V and Nickel-based Superalloy Inconel 718.

---

**👤 You:**
> "Rank these materials for the best stiffness-to-weight ratio: Aluminum 6061, Steel 1018, and Titanium Ti-6Al-4V."

**🤖 AI Agent:**
> Based on the stiffness-to-weight ratio, the ranking is: 1. Titanium Ti-6Al-4V, 2. Aluminum 6061, 3. Steel 1018.

---

**👤 You:**
> "Compare the density and yield strength of Aluminum 6061 and Steel 1018."

**🤖 AI Agent:**
> Aluminum 6061 has a density of 2.70 g/cm³ and a yield strength of 276 MPa, while Steel 1018 has a density of 7.87 g/cm³ and a yield strength of 370 MPa.


## ❓ FAQ

**Q: How do I find materials that meet my specific constraints?**
You can use the `find_suitable_materials` tool by providing a map of your required property thresholds and the expected operating conditions.

**Q: Can I optimize materials for weight reduction?**
Yes, use the `rank_materials` tool and set the performance goal to a metric like stiffness_to_weight to find the best candidates for lightweight applications.

**Q: How does the system handle manufacturing feasibility?**
The `evaluate_manufacturability_and_cost` tool provides scores for manufacturability, cost, and availability based on your intended production method, such as casting or 3d_printing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/material-selection-database](https://vinkius.com/ai-agent-connect/material-selection-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Material Selection Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `material-selection-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Material Selection Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "material-selection-database": {
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
