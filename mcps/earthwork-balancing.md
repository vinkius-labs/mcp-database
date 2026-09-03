# Earthwork Balancing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/earthwork-balancing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Optimize cut and fill volumes using mass haul analysis.

## Description
This MCP server provides advanced earthwork optimization tools. It allows AI agents to calculate material surpluses and deficits, analyze mass haul profiles, and minimize transport costs. Use `calculate_volume_balance` to determine total borrow or waste, `analyze_mass_haul` for station-by-station profiles, `optimize_haulage` to find the most efficient movement plan, and `locate_borrow_pit` to identify the best external source location.


## Available Tools (4)
- **analyze_mass_haul**: Provides a detailed breakdown of the earthwork profile to identify specific areas of surplus and deficit
- **calculate_volume_balance**: Determines the fundamental surplus or deficit of material across the entire project
- **locate_borrow_pit**: Finds the ideal external source location to minimize the cost of bringing in required material
- **optimize_haulage**: Identifies the most cost-effective movement of material to minimize total transport work


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Earthwork Balancing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total borrow and waste for a project with cut volumes [100, 200, 50] and fill volumes [150, 100, 50] with a 0.1 shrinkage factor."

**🤖 AI Agent:**
> The project requires a borrow volume of 35 m³ and has a waste volume of 0 m³.

---

**👤 You:**
> "Where should I place a borrow pit for these volumes: cut [50, 50], fill [100, 100], shrinkage 0.1, at coordinates [0, 100]?"

**🤖 AI Agent:**
> The optimal borrow pit location is at coordinate 50.0 m, with an estimated import cost of 11000.0 m³·m.

---

**👤 You:**
> "Show me the mass haul profile for cut [200, 0] and fill [0, 150] with 0.1 shrinkage."

**🤖 AI Agent:**
> The station profiles show a surplus of 200 m³ at station 0 and a deficit of 165 m³ at station 1.


## ❓ FAQ

**Q: How does the shrinkage factor affect calculations?**
The shrinkage factor accounts for the volume reduction that occurs when soil is compacted in a fill area. The tool adjusts fill requirements upward to ensure the final compacted volume meets design specifications.

**Q: Can I find the best location for a borrow pit?**
Yes, by using the `locate_borrow_pit` tool, you can identify the optimal linear coordinate to minimize the mass-distance work required to satisfy material deficits.

**Q: What is included in the haulage optimization?**
The `optimize_haulage` tool provides a complete haul plan, including specific moves from surplus stations to deficit stations and the total minimized haul work.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/earthwork-balancing](https://vinkius.com/ai-agent-connect/earthwork-balancing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Earthwork Balancing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `earthwork-balancing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Earthwork Balancing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "earthwork-balancing": {
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
