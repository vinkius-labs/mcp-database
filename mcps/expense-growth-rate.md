# Expense Growth Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/expense-growth-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate percentage changes between expense periods.

## Description
This MCP server provides tools to analyze spending fluctuations. Use `get_growth_rate` to find the exact percentage change, `get_growth_summary` for human-readable reports, `compare_expense_tiers` to categorize the intensity of changes, and `batch_growth_analysis` to evaluate multiple expense pairs at once.


## Available Tools (4)
- **batch_growth_analysis**: Evaluates a list of historical expense changes to find the highest and lowest growth points
- **compare_expense_tiers**: Categorizes the magnitude of the growth rate into qualitative tiers
- **get_growth_rate**: Calculates the percentage increase or decrease between a previous expense amount and a current expense amount
- **get_growth_summary**: Provides a descriptive text-based interpretation of the growth change for reporting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expense Growth Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the growth rate if last month's expense was 100 and this month's is 125?"

**🤖 AI Agent:**
> The growth rate is 0.25, which represents a 25% increase.

---

**👤 You:**
> "Give me a summary of the change from 500 to 450."

**🤖 AI Agent:**
> Expenses decreased by 10%.

---

**👤 You:**
> "Categorize the growth from 1000 to 1500."

**🤖 AI Agent:**
> The change is categorized as Significant.


## ❓ FAQ

**Q: How do I calculate the growth rate?**
You can use the `get_growth_rate` tool by providing the base expense and the current expense.

**Q: Can I analyze multiple expense changes at once?**
Yes, the `batch_growth_analysis` tool allows you to evaluate a list of historical expense pairs.

**Q: What happens if the base expense is zero?**
The tools will return an error to prevent division by zero, as a base expense must be greater than zero.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/expense-growth-rate](https://vinkius.com/en/ai-agent-connect/expense-growth-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expense Growth Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `expense-growth-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expense Growth Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expense-growth-rate": {
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
