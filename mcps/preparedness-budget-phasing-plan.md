# Preparedness Budget Phasing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/preparedness-budget-phasing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A strategic financial engine that transforms emergency readiness gaps into a month-by-month procurement roadmap.

## Description
This MCP server provides a suite of financial planning tools to help users prepare for emergencies without incurring debt. It transforms a list of readiness gaps into a structured, chronological purchasing plan. Users can use `generate_phasing_plan` to create a monthly roadmap, `analyze_readiness_feasibility` to check if their goals are mathematically possible, and `validate_budget_constraint` to ensure individual purchases respect their emergency fund targets and no-debt rules. It is designed to protect liquidity while systematically addressing critical safety needs.


## Available Tools (4)
- **analyze_readiness_feasibility**: Determines if the user's goals are mathematically possible given their budget and timeline
- **generate_phasing_plan**: Generates the complete step-by-step procurement roadmap based on user constraints
- **get_spending_record_template**: Provides a structured format for the user to track actual vs. planned spending
- **validate_budget_constraint**: Checks if a specific item purchase violates the user's established financial rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Preparedness Budget Phasing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a purchasing plan for a water filter ($150) and a medical kit ($200). My monthly budget is $50, my emergency fund target is $1000, and I want to finish by December."

**🤖 AI Agent:**
> Your procurement plan is ready. You will purchase the water filter in Month 1 and the medical kit in Month 4 to stay within your $50 monthly budget while maintaining your emergency fund.

---

**👤 You:**
> "Is it possible to buy all my readiness items for $500 total if I have a $50 monthly budget and a target date of 3 months from now?"

**🤖 AI Agent:**
> No, with a $50 monthly budget over 3 months, you can only afford $150. You will have a gap of $350 to meet your $500 goal.

---

**👤 You:**
> "I want to buy a solar generator for $400. My current savings are $1200, my target is $1000, and my monthly budget is $100. Can I afford this now?"

**🤖 AI Agent:**
> No, purchasing the solar generator now would reduce your savings to $800, which is below your $1000 emergency fund target.


## ❓ FAQ

**Q: How does the phasing plan work?**
The `generate_phasing_plan` tool takes your list of items, their prices, and your monthly budget to create a month-by-month schedule that prioritizes items based on their urgency tier.

**Q: Can I ensure I don't go into debt?**
Yes. By using the `applyNoDebtRule` parameter in the planning tools, the engine ensures no purchase is made that would drop your savings below your specified emergency fund target.

**Q: How can I track my actual spending against the plan?**
You can use the `get_spending_record_template` tool to generate a structured format for tracking planned versus actual costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/preparedness-budget-phasing-plan](https://vinkius.com/en/ai-agent-connect/preparedness-budget-phasing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Preparedness Budget Phasing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `preparedness-budget-phasing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Preparedness Budget Phasing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "preparedness-budget-phasing-plan": {
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
