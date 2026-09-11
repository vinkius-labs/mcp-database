# Infra Unit Economics & Gross Margin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/infra-unit-economics-gross-margin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate gross margin, cost breakdowns, and identify margin improvement levers for infrastructure businesses.

## Description
This MCP server provides specialized financial analysis tools for infrastructure-heavy businesses. It allows AI agents to calculate gross margin percentages, analyze cost distributions across maintenance, energy, labor, and depreciation, and identify specific levers to improve profitability. Use `calculate_gross_margin` to determine total COGS and margin, `analyze_cost_breakdown` to see cost distribution, `identify_margin_levers` to find optimization opportunities, and `validate_infrastructure_health` to compare current margins against target thresholds.


## Available Tools (4)
- **analyze_cost_breakdown**: Analyze cost distribution across categories
- **calculate_gross_margin**: Calculate gross margin and total COGS
- **identify_margin_levers**: Identify primary cost levers for margin improvement
- **validate_infrastructure_health**: Validate infrastructure margin health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infra Unit Economics & Gross Margin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current gross margin if revenue is $1,000,000, maintenance is $100,000, energy is $150,000, labor is $200,000, and depreciation is $50,000?"

**🤖 AI Agent:**
> Your total COGS is $500,000 and your current gross margin is 50.0%.

---

**👤 You:**
> "Analyze my cost distribution with maintenance at $50,000, energy at $80,000, labor at $40,000, and depreciation at $30,000."

**🤖 AI Agent:**
> Energy is your largest cost component at 40%, followed by maintenance at 25%, labor at 20%, and depreciation at 15%.

---

**👤 You:**
> "Is my margin healthy if it is 25% and my target is 30%?"

**🤖 AI Agent:**
> No, your current margin is below the target. The variance is -5.0%.


## ❓ FAQ

**Q: What is included in the COGS calculation?**
The total Cost of Goods Sold (COGS) includes maintenance costs, energy costs, direct labor, and depreciation amounts.

**Q: How can I find ways to improve my profit margins?**
You can use the `identify_margin_levers` tool to pinpoint which cost categories are most significant and offer the best opportunities for reduction.

**Q: Can I check if my business is meeting its financial targets?**
Yes, the `validate_infrastructure_health` tool compares your current gross margin against a target margin to determine if your operations are healthy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/infra-unit-economics-gross-margin](https://vinkius.com/en/ai-agent-connect/infra-unit-economics-gross-margin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infra Unit Economics & Gross Margin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-unit-economics-gross-margin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infra Unit Economics & Gross Margin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-unit-economics-gross-margin": {
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
