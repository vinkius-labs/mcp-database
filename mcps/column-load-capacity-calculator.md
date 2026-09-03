# Column Load Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/column-load-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate axial load, moment capacity, and slenderness for reinforced concrete columns.

## Description
This MCP server provides structural engineering tools to analyze reinforced concrete columns. It calculates axial load capacity, moment capacity, and evaluates buckling risks using the `get_capacity_summary` tool. It accounts for concrete strength, steel reinforcement, eccentricity, and slenderness effects to provide accurate design values.


## Available Tools (4)
- **get_axial_capacity**: Calculates the total axial load capacity of the column
- **get_capacity_summary**: Provides a comprehensive overview of the column's structural performance
- **get_moment_capacity**: Determines the maximum bending moment the column can resist
- **get_slenderness_ratio**: Evaluates the geometric risk of buckling


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Column Load Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the axial capacity of a 300x300mm column with 30MPa concrete and 1200mm2 steel?"

**🤖 AI Agent:**
> The axial capacity for the specified column is 1450 kN with a reduction factor of 0.85.

---

**👤 You:**
> "Check the slenderness of a column that is 200mm wide, 400mm deep, and 3m effective length."

**🤖 AI Agent:**
> The slenderness ratio is 15.2, and the column is classified as non-slender.

---

**👤 You:**
> "Give me a full capacity summary for a 400x400mm column, 35MPa concrete, 1500mm2 steel, 450MPa steel, 3.5m length, and 50mm eccentricity."

**🤖 AI Agent:**
> Summary: Axial Capacity is 1820 kN, Moment Capacity is 115 kNm, Reduction Factor is 0.78, and Slenderness Ratio is 18.5.


## ❓ FAQ

**Q: What can this tool calculate?**
It calculates axial capacity, moment capacity, slenderness ratio, and provides a full structural summary using `get_capacity_summary`.

**Q: How does eccentricity affect the results?**
Eccentricity introduces bending moments, which reduces the pure axial load capacity. The tools account for this offset.

**Q: Does it account for buckling?**
Yes, the `get_slenderness_ratio` tool evaluates the geometric risk of buckling based on the effective length and column dimensions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/column-load-capacity-calculator](https://vinkius.com/ai-agent-connect/column-load-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Column Load Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `column-load-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Column Load Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "column-load-capacity-calculator": {
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
