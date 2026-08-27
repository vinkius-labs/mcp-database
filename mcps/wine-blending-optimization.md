# Wine Blending Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-blending-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate ideal wine proportions to meet chemical targets and budget constraints.

## Description
This MCP server provides advanced mathematical optimization for wine blending. It allows AI agents to calculate the precise proportions of component wines needed to hit specific chemical targets--such as alcohol, pH, and tannins--while strictly adhering to volume and budget constraints. Using tools like `find_optimal_blend` and `simulate_blend_quality`, you can determine the most cost-effective mixtures or verify the chemical profile of a proposed blend before production.


## Available Tools (4)
- **evaluate_constraint_viability**: Determines if it is mathematically possible to meet a set of targets given available wines and a budget
- **find_optimal_blend**: , while staying under a budget.

Calculates the best proportions for a wine blend to meet chemical targets within a budget
- **get_component_summary**: Provides a quick overview of available component wines for selection
- **simulate_blend_quality**: Predicts the chemical profile of a specific, user-defined set of wine proportions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Blending Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best blend for 1000 liters of wine with alcohol between 13% and 14%, with a max budget of 5000."

**🤖 AI Agent:**
> The optimal blend for 1000 liters requires 450L of Wine A and 550L of Wine B, resulting in 13.5% alcohol at a total cost of 4850.

---

**👤 You:**
> "What will the alcohol content be if I mix 200L of Wine X (12% alcohol) and 300L of Wine Y (15% alcohol)?"

**🤖 AI Agent:**
> The resulting blend will have an alcohol content of 13.8% and a total volume of 500L.

---

**👤 You:**
> "List all available wines that cost less than 5 per liter."

**🤖 AI Agent:**
> The available wines under 5 per liter are: Wine_001, Wine_004, and Wine_009.


## ❓ FAQ

**Q: How can I find the best mixture for a specific target?**
You can use the `find_optimal_blend` tool. Provide the list of available component wines, your target chemical ranges, the desired total volume, and your maximum budget.

**Q: Can I check if my targets are even possible?**
Yes, use `evaluate_constraint_viability` to determine if a valid solution exists within your budget and chemical constraints before attempting to optimize.

**Q: How do I see the chemical profile of a specific blend?**
Use the `simulate_blend_quality` tool by providing the component wines and the specific volumes you wish to test.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-blending-optimization](https://vinkius.com/ai-agent-connect/wine-blending-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Blending Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-blending-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Blending Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-blending-optimization": {
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
