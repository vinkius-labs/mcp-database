# Income Statement Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/income-statement-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate structured Income Statements (P&L) with vertical analysis.

## Description
Transform raw financial data into a professional, hierarchical Income Statement. This tool automates the calculation of Net Revenue, Gross Profit, EBIT, EBT, and Net Income using vertical analysis to show each line item as a percentage of revenue. Use `generate_income_statement` for full reports, `calculate_profitability_margins` for margin health diagnostics, and `analyze_expense_composition` to identify cost drivers.


## Available Tools (3)
- **analyze_expense_composition**: Identifies which expense categories are the primary drivers of cost
- **calculate_profitability_margins**: Provides a quick diagnostic of the company's margin health
- **generate_income_statement**: Produces a complete, hierarchical Income Statement (P/L) with vertical analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Income Statement Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an income statement with $100,000 gross revenue, $5,000 deductions, $40,000 COGS, $20,000 SG&A, $2,000 financial results, and $3,000 taxes."

**🤖 AI Agent:**
> The Income Statement has been generated. Net Revenue: $95,000 (100%), Gross Profit: $55,000 (57.89%), EBIT: $35,000 (36.84%), EBT: $33,000 (34.74%), Net Income: $30,000 (31.58%).

---

**👤 You:**
> "What are my profit margins for a company with $50,000 revenue and $10,000 net income?"

**🤖 AI Agent:**
> Based on the provided data, your Net Margin is 20%.

---

**👤 You:**
> "Show me the breakdown of my expenses."

**🤖 AI Agent:**
> The expense composition analysis shows that COGS accounts for 60% of total expenses, while SG&A accounts for 35%.


## ❓ FAQ

**Q: What is vertical analysis?**
Vertical analysis expresses each line item on the Income Statement as a percentage of Net Revenue, allowing for easy comparison across different periods.

**Q: How do I use `calculate_profitability_margins`?**
Provide your gross revenue, deductions, COGS, and other expenses. The tool will return your Gross, Operating, and Net margins.

**Q: Can I analyze specific expense drivers?**
Yes, use the `analyze_expense_composition` tool to see how much each category like COGS or SG&A contributes to your total expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/income-statement-generator](https://vinkius.com/mcp/income-statement-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Income Statement Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `income-statement-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Income Statement Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "income-statement-generator": {
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
