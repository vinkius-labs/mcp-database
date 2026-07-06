# Concrete Material Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/concrete-material-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Estimate concrete volume, bag quantities, costs, and rebar requirements for any project.

## Description
The Concrete Material Calculator is an engineering utility designed to simplify material estimation for construction projects. Whether you are pouring a simple slab, structural footings, vertical columns, or complex staircases, this tool provides precise calculations for volume in both cubic yards and cubic meters. It also calculates the exact number of 40lb, 60lb, and 80lb pre-mixed bags required, along with an estimated cost estimate to help you budget effectively. Additionally, use `query_rebar_quantity` to determine the total pieces and linear footage of rebar needed for your reinforcement grid. This tool accounts for waste percentages to ensure you never run short during a pour.


## Available Tools (6)
- **query_column_materials**: Calculates materials for cylindrical or square vertical columns
- **query_curved_surface_materials**: Calculates materials for irregular or curved surfaces
- **query_footing_materials**: Calculates materials for linear trench footings
- **query_rebar_quantity**: Calculates the amount of rebar needed for a specific slab or footing area
- **query_slab_materials**: Calculates materials for flat, area-based surfaces like slabs or countertops
- **query_step_materials**: Calculates materials for a multi-step staircase structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Material Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 80lb bags of concrete do I need for a slab that is 10ft wide, 12ft long, and 4 inches thick with 10% waste?"

**🤖 AI Agent:**
> You will need approximately 18 bags of 80lb concrete for this slab.

---

**👤 You:**
> "Calculate materials for a footing trench that is 2ft wide, 1ft deep, and 50ft long with 5% waste."

**🤖 AI Agent:**
> The total volume required is approximately 3.15 cubic yards, which translates to roughly 42 bags of 80lb concrete.

---

**👤 You:**
> "How much rebar do I need for a 10x10 area with 12-inch spacing and 6 inches of overlap?"

**🤖 AI Agent:**
> You will need 22 pieces of rebar, totaling 220 linear feet.


## ❓ FAQ

**Q: How does the calculator handle waste?**
The tool allows you to input a `wastePercentage` for every calculation. This ensures that your final volume includes a buffer for uneven subgrades, spillage, or formwork deflection.

**Q: Can I calculate rebar needs alongside concrete?**
Yes, by using the `query_rebar_quantity` tool, you can input your area dimensions and spacing to get the total number of pieces and linear feet required for reinforcement.

**Q: Does it support metric measurements?**
Absolutely. Most tools include a `useMetric` parameter that allows you to switch between imperial (feet/inches) and metric (meters/cm) systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/concrete-material-calculator](https://vinkius.com/mcp/concrete-material-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Material Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-material-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Material Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-material-calculator": {
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
