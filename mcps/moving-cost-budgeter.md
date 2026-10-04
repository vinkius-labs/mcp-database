# Moving Cost Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-cost-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and analyze moving expenses across upfront, move-week, and first-month phases.

## Description
This MCP server provides specialized tools to manage relocation finances. It categorizes expenses into three temporal phases: Upfront, Move-Week, and First-Month. Users can use `get_budget_summary` to see core totals, `calculate_phase_breakdown` to analyze phase concentration, `validate_contingency_buffer` to ensure financial safety, and `get_category_analysis` to identify primary cost drivers.


## Available Tools (4)
- **get_budget_summary**: Provides the three core financial totals for the moving plan
- **get_category_analysis**: Optionally specify sort order (ascending or descending).

Answers which specific service is driving the budget
- **validate_contingency_buffer**: Checks if the allocated contingency fund is sufficient based on the total weight of other expenses
- **calculate_phase_breakdown**: Answers how much of the total budget is concentrated in a specific time period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Cost Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my moving budget."

**🤖 AI Agent:**
> Your upfront total is $500, your move-week total is $1,200, and your first-month total is $300.

---

**👤 You:**
> "What percentage of my budget is spent during the move-week?"

**🤖 AI Agent:**
> The move-week phase represents 60% of your total budget.

---

**👤 You:**
> "Is my 10% contingency buffer sufficient?"

**🤖 AI Agent:**
> No, you have a shortfall of $150 to meet your 10% buffer requirement.


## ❓ FAQ

**Q: How are the totals calculated?**
Totals are aggregated using `get_budget_summary` based on the temporal phases: Upfront, Move-Week, and First-Month.

**Q: Can I check if my emergency fund is enough?**
Yes, you can use `validate_contingency_buffer` to check if your contingency amount meets your required buffer percentage.

**Q: How do I see which category costs the most?**
Use the `get_category_analysis` tool to get a ranked list of your expense categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-cost-budgeter](https://vinkius.com/en/ai-agent-connect/moving-cost-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Cost Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-cost-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Cost Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-cost-budgeter": {
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
