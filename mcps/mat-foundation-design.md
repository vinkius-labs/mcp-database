# mat-foundation-design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mat-foundation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for mat foundation thickness, reinforcement, and settlement calculations.

## Description
This MCP server provides specialized engineering tools for designing mat foundations. It allows AI agents to perform critical structural calculations including `analyze_foundation_geometry` to verify layout feasibility, `calculate_mat_thickness` for slab depth requirements, `estimate_settlement` to predict vertical soil movement, and `design_reinforcement` to determine steel patterns. The tool accounts for soil-structure interaction and edge effects to ensure structural integrity.


## Available Tools (4)
- **calculate_mat_thickness**: Determine the required slab thickness based on structural requirements
- **design_reinforcement**: Generate the required steel reinforcement pattern for the slab
- **estimate_settlement**: Predict the vertical movement of the foundation into the soil
- **analyze_foundation_geometry**: Validate the physical feasibility of the foundation dimensions and column layout


## 💬 Prompt Examples

Here are some examples of how you can interact with the **mat-foundation-design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a 10m x 10m mat with a column at (5,5) carrying 500kN is feasible."

**🤖 AI Agent:**
> The foundation geometry is feasible. The total area is 100 square meters and the load center is at (5, 5).

---

**👤 You:**
> "What is the required thickness for a 15m x 15m mat with 1000kN loads and 30MPa concrete?"

**🤖 AI Agent:**
> The required thickness is 450 mm, and the punching shear check passed.

---

**👤 You:**
> "Estimate the settlement for a 20m x 20m mat on soil with 150kPa capacity and 2000kN total load."

**🤖 AI Agent:**
> The estimated total settlement is 25 mm and the differential settlement is 8 mm.


## ❓ FAQ

**Q: How do I verify if my column layout is valid?**
You can use the `analyze_foundation_geometry` tool. It checks if the column positions fall within the specified mat dimensions and ensures the total load is non-zero.

**Q: Can this tool predict soil settlement?**
Yes, the `estimate_settlement` tool predicts both total and differential settlement by accounting for soil-structure interaction.

**Q: Does the tool calculate reinforcement requirements?**
Yes, the `design_reinforcement` tool generates the required steel area and spacing for the slab based on the provided thickness and soil bearing capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mat-foundation-design](https://vinkius.com/ai-agent-connect/mat-foundation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **mat-foundation-design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mat-foundation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **mat-foundation-design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mat-foundation-design": {
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
