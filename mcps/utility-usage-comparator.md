# Utility Usage Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/utility-usage-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare monthly utility bills against historical trends and household occupancy.

## Description
This MCP server provides tools to analyze utility expenses for electricity, water, gas, and internet. It calculates absolute and per-person changes in cost and consumption, identifies cost drivers like usage or rate changes, and provides annual expenditure projections. Use `compare_utility_usage` to evaluate specific billing periods or `summarize_utility_trends` to see a household-wide overview.


## Available Tools (4)
- **project_annual_cost**: Predicts the total yearly expenditure for a specific utility
- **compare_utility_usage**: Analyzes the difference in cost and consumption between the current bill and a baseline period
- **summarize_utility_trends**: Provides a high-level overview of trends across multiple utility types
- **get_occupancy_impact_report**: Calculates how changes in household size have specifically affected the utility burden


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Utility Usage Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare my electricity usage. Current: $150, 500kWh, 4 people. Baseline: $120, 450kWh, 4 people."

**🤖 AI Agent:**
> The absolute amount change is $30.00, and the absolute consumption change is 50kWh. The per-person amount change is $7.50.

---

**👤 You:**
> "Predict my annual gas cost if I spent $80 this month."

**🤖 AI Agent:**
> The projected annual total for gas is $960.00 (confidence level: low).

---

**👤 You:**
> "Summarize my utility trends for electricity ($100 current, $80 baseline, 40kWh current, 35kWh baseline, 2 people current, 2 people baseline) and water ($50 current, $40 baseline, 10 units current, 8 units baseline, 2 people current, 2 people baseline)."

**🤖 AI Agent:**
> The total household spend trend is $30.00. The most volatile utility is electricity. The average per-person trend is $12.50.


## ❓ FAQ

**Q: How do I compare my current electricity bill to last month?**
You can use the `compare_utility_usage` tool by providing the current and baseline period data, including amount, consumption, and occupancy.

**Q: Can I predict my yearly water costs?**
Yes, the `project_annual_cost` tool allows you to estimate your total yearly expenditure based on your current monthly amount.

**Q: How does household size affect my utility analysis?**
The tool uses occupancy to calculate per-person metrics, helping you understand if cost changes are due to more people in the house or increased individual usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/utility-usage-comparator](https://vinkius.com/en/ai-agent-connect/utility-usage-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Utility Usage Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `utility-usage-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Utility Usage Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "utility-usage-comparator": {
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
