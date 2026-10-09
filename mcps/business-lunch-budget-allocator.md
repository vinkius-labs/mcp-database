# Business Lunch Budget Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/business-lunch-budget-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise per-person food budgets while accounting for tax, tip, and monthly limits.

## Description
This MCP server provides an intelligent allocation engine for managing client meal expenses. It helps users determine exactly how much can be spent on menu items by calculating the impact of taxes and tips against a fixed meal cap. Use `optimize_per_person_food_budget` to find the raw food budget per person, `check_single_lunch_feasibility` to verify if a specific group size fits a budget, and `calculate_monthly_budget_impact` to ensure a series of lunches stays within monthly limits.


## Available Tools (4)
- **calculate_monthly_budget_impact**: Checks if a planned series of lunches will exceed the total monthly budget
- **check_single_lunch_feasibility**: Determines if a specific lunch configuration is possible within a single meal cap
- **optimize_per_person_food_budget**: Calculates the exact amount available for menu items per person
- **validate_lunch_frequency**: Checks if the proposed frequency of meetings is compatible with the monthly budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Lunch Budget Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a $200 meal cap for 4 people. Tax is 8% and tip is 20%. How much can we spend on food per person?"

**🤖 AI Agent:**
> With a $200 cap for 4 people, the food budget per person is $133.33. This leaves $66.67 for tax and tip.

---

**👤 You:**
> "Will 4 lunches at $150 each fit in my $500 monthly budget?"

**🤖 AI Agent:**
> No, 4 lunches at $150 each would cost $600, which exceeds your $500 monthly budget by $100.

---

**👤 You:**
> "Check if a $100 lunch for 2 people is possible with 10% tax and 15% tip."

**🤖 AI Agent:**
> Yes, a $100 lunch for 2 people is feasible. The total projected cost is $100.00.


## ❓ FAQ

**Q: How does the tool handle taxes and tips?**
The tool subtracts the calculated tax and tip amounts from the total meal cap to determine the remaining budget available for actual food items.

**Q: Can I check if my monthly budget is sufficient for weekly lunches?**
Yes, you can use `calculate_monthly_budget_impact` to see if your planned frequency of lunches will exceed your total monthly funds.

**Q: What happens if I have a large group of attendees?**
The tool uses `check_single_lunch_feasibility` to ensure that the attendee count, combined with tax and tip, does not exceed your specified meal cap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/business-lunch-budget-allocator](https://vinkius.com/en/ai-agent-connect/business-lunch-budget-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Lunch Budget Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-lunch-budget-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Lunch Budget Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-lunch-budget-allocator": {
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
