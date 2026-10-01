# Seedling Thinning & Spacing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seedling-thinning-spacing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate exact seedling removal and retention counts for optimal plant spacing.

## Description
This MCP server provides precise agricultural calculations to manage plant density. It helps growers determine exactly how many seedlings to remove and how many to retain to achieve a target spacing. Use `get_thinning_summary` for a high-level overview across all rows, `get_row_specific_plan` for detailed individual row requirements, `validate_spacing_viability` to check if a proposed spacing is feasible, and `get_density_metrics` to compare plant density levels.


## Available Tools (4)
- **get_row_specific_plan**: Calculates the exact thinning requirements for a single specific row
- **get_thinning_summary**: Provides a high-level overview of how many plants to keep and how many to remove across all rows
- **validate_spacing_viability**: Determines if a proposed target spacing is biologically or physically feasible given the current setup
- **get_density_metrics**: Calculates the plant density for comparison between current and target states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seedling Thinning & Spacing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 10 rows, each 50 meters long. Current spacing is 0.1m and I want 0.2m. How many plants should I remove in total?"

**🤖 AI Agent:**
> You should remove 2,000 seedlings in total to achieve the target spacing.

---

**👤 You:**
> "Is a target spacing of 0.05m viable if my current spacing is 0.1m and the minimum allowed is 0.08m?"

**🤖 AI Agent:**
> No, the proposed spacing is not viable because it is less than the minimum allowed spacing of 0.08m.

---

**👤 You:**
> "Calculate the density for a 100m row with 0.25m spacing."

**🤖 AI Agent:**
> The plant density is 4.0 plants per meter.


## ❓ FAQ

**Q: How do I know how many plants to remove?**
You can use the `get_thinning_summary` tool to get the total number of seedlings to remove across all your rows based on your current and target spacing.

**Q: Can I check if my target spacing is valid?**
Yes, the `validate_spacing_viability` tool checks if your proposed spacing meets the minimum requirements for your specific crop.

**Q: Does this work for individual rows?**
Yes, use `get_row_specific_plan` to calculate the exact number of seedlings to retain or remove for a single specific row.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seedling-thinning-spacing-plan](https://vinkius.com/en/ai-agent-connect/seedling-thinning-spacing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seedling Thinning & Spacing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seedling-thinning-spacing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seedling Thinning & Spacing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seedling-thinning-spacing-plan": {
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
