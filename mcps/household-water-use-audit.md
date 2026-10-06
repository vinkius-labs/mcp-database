# Household Water Use Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-water-use-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate residential water consumption, leak impacts, and monthly projections.

## Description
This MCP server provides a complete toolkit for auditing residential water consumption. It allows AI agents to calculate total daily usage from fixture flow rates, generate detailed daily reports including per-person averages, project monthly water needs, and analyze the severity of water leaks. Use `get_fixture_usage_summary` to aggregate consumption by category, `get_household_daily_report` for a full daily snapshot, `get_monthly_projections` for budgeting, and `get_leak_impact_analysis` to evaluate waste severity.


## Available Tools (4)
- **get_household_daily_report**: Generates a complete daily snapshot including functional usage, leakages, and per-person averages
- **get_fixture_usage_summary**: Calculates the total water consumed by specific categories of fixtures based on their flow rates and usage patterns
- **get_leak_impact_analysis**: Analyzes how much water is being lost specifically due to continuous leaks versus standard usage
- **get_monthly_projections**: Extrapolates daily usage patterns into a monthly view for budgeting or resource planning


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Water Use Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my daily water usage for a house with 4 people. I have a shower (10L/min, 10 mins, 2 uses/day) and a toilet (6L/use, 4 uses/day). There is a leak of 5L per day."

**🤖 AI Agent:**
> Your total daily water usage is 245 liters, with a per-person average of 61.25 liters.

---

**👤 You:**
> "Based on a daily usage of 300 liters, what is my projected usage for a 31-day month?"

**🤖 AI Agent:**
> Your projected monthly total is 9,300 liters.

---

**👤 You:**
> "I am losing 50 liters a day to a leak. My fixtures use 200 liters a day. How bad is the leak?"

**🤖 AI Agent:**
> The leak severity is Medium, with a leak-to-usage ratio of 0.25.


## ❓ FAQ

**Q: How do I calculate my total daily water usage?**
You can use the `get_fixture_usage_summary` tool to calculate usage based on your fixtures, and then use `get_household_daily_report` to include any detected leak volumes for a final daily total.

**Q: Can I estimate my monthly water bill?**
Yes, by using the `get_monthly_projections` tool with your current daily total and the number of days in the month.

**Q: How does the tool identify water leaks?**
The `get_leak_impact_analysis` tool compares your daily leak volume against your functional fixture usage to determine a waste severity level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-water-use-audit](https://vinkius.com/en/ai-agent-connect/household-water-use-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Water Use Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-water-use-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Water Use Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-water-use-audit": {
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
