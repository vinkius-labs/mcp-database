# Blending Optimization Mining MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/blending-optimization-mining)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimize ore blending using linear programming to meet grade constraints and maximize value.

## Description
This MCP server provides advanced mathematical tools for metallurgical blending. It allows AI agents to solve complex linear programming problems to find the most efficient combination of ore sources. By using `get_source_availability`, agents can inspect current stockpiles, and with `calculate_optimal_blend`, they can generate precise recipes that satisfy specific grade constraints for mass and quality. It also includes `validate_blend_feasibility` to check if a target is achievable and `predict_blend_quality` to forecast the chemical composition of a proposed mix.


## Available Tools (4)
- **get_source_availability**: Retrieves current stock levels and quality profiles for all available ore stockpiles
- **predict_blend_quality**: Calculates the expected chemical composition of a blend given a specific allocation of ore masses
- **validate_blend_feasibility**: Quickly checks if a specific combination of ore sources can theoretically meet the required grade constraints
- **calculate_optimal_blend**: Solves the linear programming problem to find the most efficient combination of ore sources to meet grade constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blending Optimization Mining** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best blend for 5000 tons of ore with at least 62% Iron and max 0.05% Phosphorus using available sources."

**🤖 AI Agent:**
> The optimal recipe for 5000 tons is: Source_A (3200 tons) and Source_B (1800 tons), resulting in 62.5% Iron and 0.04% Phosphorus.

---

**👤 You:**
> "Is it possible to blend 1000 tons of ore with 65% Iron using the current stockpiles?"

**🤖 AI Agent:**
> No, the current stockpiles cannot reach a 65% Iron concentration for a 1000 ton mass; the maximum achievable is 63.8%.

---

**👤 You:**
> "What will the quality be if I mix 2000 tons of Source_A and 3000 tons of Source_C?"

**🤖 AI Agent:**
> The predicted blend will have a total mass of 5000 tons with an Iron grade of 61.2% and Silica content of 4.5%.


## ❓ FAQ

**Q: How can I find the best ore recipe?**
You can use the `calculate_optimal_blend` tool to find the most efficient combination of sources based on your target mass and grade constraints.

**Q: Can I check if my desired blend is possible?**
Yes, the `validate_blend_feasibility` tool allows you to verify if a specific set of ore sources can meet your required quality parameters.

**Q: Where can I see available ore stockpiles?**
Use the `get_source_availability` tool to retrieve current stock levels, costs, and chemical profiles for all available ore sources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/blending-optimization-mining](https://vinkius.com/ai-agent-connect/blending-optimization-mining)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blending Optimization Mining** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blending-optimization-mining` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blending Optimization Mining** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blending-optimization-mining": {
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
