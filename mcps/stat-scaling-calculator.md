# Stat Scaling Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stat-scaling-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Compute and compare attribute progression curves for game design.

## Description
This MCP server provides game designers with precise mathematical tools to define how attributes like Strength, Health, or Mana evolve from Level 1 to a maximum level. Using `compute_progression_table`, you can generate detailed level-by-level breakdowns for various growth archetypes including linear, exponential, and S-curves. The `analyze_growth_velocity` tool helps identify unintended power spikes by calculating the delta between levels, while `compare_scaling_strategies` allows for a unified visual comparison of multiple scaling configurations to ensure consistent progression feel.


## Available Tools
- **compare_scaling_strategies**: Produces a unified dataset for visual comparison of different scaling configurations
- **analyze_growth_velocity**: Calculates the incremental change in an attribute's value between consecutive levels
- **compute_progression_table**: Generates a complete step-by-step breakdown of an attribute's value for every level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stat Scaling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a linear progression table from 10 to 100 up to level 50."

**🤖 AI Agent:**
> The `compute_progression_table` tool will generate a breakdown where each level increases by exactly 1.837...

---

**👤 You:**
> "Analyze the growth velocity of this table: [{"level": 1, "statValue": 10}, {"level": 2, "statValue": 15}]"

**🤖 AI Agent:**
> The `analyze_growth_velocity` tool shows a delta of 5 at level 2.

---

**👤 You:**
> "Compare an exponential curve (10 to 500, lvl 20) with a linear curve (10 to 500, lvl 20)."

**🤖 AI Agent:**
> The `compare_scaling_strategies` tool will provide a unified dataset for visual comparison.


## ❓ FAQ

**Q: How can I generate a level-by-level attribute breakdown?**
Use the `compute_progression_table` tool by providing your base stat, target stat, maximum level, and desired curve type.

**Q: How do I identify power spikes in my progression?**
The `analyze_growth_velocity` tool calculates the change in value between consecutive levels, making it easy to spot sudden jumps or plateaus.

**Q: Can I compare different scaling archetypes side-by-side?**
Yes. The `compare_scaling_strategies` tool aligns multiple configurations onto a single dataset for direct comparison.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stat-scaling-calculator](https://vinkius.com/mcp/stat-scaling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stat Scaling Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stat-scaling-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stat Scaling Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stat-scaling-calculator": {
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
