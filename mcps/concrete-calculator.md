# Concrete Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Deterministic tool for precise concrete volume, material, and rebar calculations.

## Description
This MCP server provides precise, deterministic calculations for all concrete-related structural needs. Use `calculate_volume` to determine the total volume required for slabs, footings, piers, or walls, including a customizable waste safety margin. Use `estimate_materials` to calculate the exact number of bags needed for small jobs or the number of truckloads for larger pours, along with the specific weight of cement, sand, gravel, and water for on-site mixing. Finally, use `calculate_rebar` to determine the total weight and length of steel reinforcement required based on your spacing and bar diameter.


## Available Tools (3)
- **calculate_rebar**: Calculates the total weight and length of steel reinforcement required
- **calculate_volume**: Determines the total required concrete volume including a waste safety margin
- **estimate_materials**: Calculates the quantity of bags or truckloads needed, and the weight of raw materials for mixing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much concrete do I need for a 10x10x0.5 foot slab with a 5% waste factor?"

**🤖 AI Agent:**
> You will need 1.58 cubic yards of concrete for that slab.

---

**👤 You:**
> "How many 80lb bags of concrete do I need for 2 cubic yards of 3000 PSI mix?"

**🤖 AI Agent:**
> You will need 68 bags of 80lb concrete.

---

**👤 You:**
> "Calculate the rebar needed for a volume of 5 cubic yards with 12 inch spacing and 0.5 inch diameter bars."

**🤖 AI Agent:**
> The total reinforcement required is 125 feet of rebar with a total weight of 25.5 lbs.


## ❓ FAQ

**Q: How does the tool handle waste?**
The `calculate_volume` tool includes a waste factor parameter, allowing you to add a safety margin (typically 5-10%) to the theoretical volume to account for spillage or uneven surfaces.

**Q: Can I calculate materials for on-site mixing?**
Yes, by using `estimate_materials` with the 'bagged' delivery method or by reviewing the raw material weights (cement, sand, gravel, water) provided in the output.

**Q: What foundation types are supported?**
The tool supports calculations for slabs, footings, piers, and walls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-calculator](https://vinkius.com/ai-agent-connect/concrete-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-calculator": {
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
