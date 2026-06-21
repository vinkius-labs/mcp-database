# Burn Rate Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/burn-rate-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze startup burn rate, expense composition, and runway forecasting.

## Description
The Burn Rate Analyzer is a financial diagnostic tool designed for startups to monitor monthly expenditure distribution and operational efficiency. Using tools like `analyze_expense_composition`, you can break to breakdown costs across categories such as salaries, infrastructure, and marketing. The `compare_stage_benchmarks` tool allows you to evaluate your spending against industry standards for Seed, Series A, or Series B stages, identifying high overhead areas. Additionally, use `calculate_runway_forecast` to determine how many months of operation remain based on your current cash reserves and monthly burn rate.


## Available Tools
- **compare_stage_benchmarks**: Evaluates the company's spending distribution against standard industry benchmarks
- **analyze_expense_composition**: Analyzes the distribution of expenses across all categories and calculates efficiency ratios
- **calculate_runway_forecast**: Determines how many months of operation remain based on current cash reserves and burn rate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burn Rate Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my expenses: salaries 50000, marketing 20000, infrastructure 10000. My revenue is 30000 and I have 5 employees."

**🤖 AI Agent:**
> The analysis shows a total burn of 80,000. Your burn per employee is 16,000, and your burn per revenue dollar is 2.67.

---

**👤 You:**
> "How much runway do I have left with 500,000 in reserves and a monthly burn of 40,000?"

**🤖 AI Agent:**
> Based on your current cash reserves and burn rate, you have approximately 12.5 months of runway remaining.

---

**👤 You:**
> "Compare my current composition (salaries: 0.7, marketing: 0.2, infrastructure: 0.1) against the Seed stage benchmark."

**🤖 AI Agent:**
> The comparison shows your spending is on track for a Seed stage startup with no significant deviations detected.


## ❓ FAQ

**Q: What metrics can I calculate with this MCP?**
You can calculate expense composition by category, burn per employee, burn per dollar of revenue, and estimated months of runway remaining.

**Q: How does the benchmarking feature work?**
The `compare_stage_benchmarks` tool compares your current expense percentages against industry standard benchmarks for Seed, Series A, and Series B stages.

**Q: Can I track specific expense categories?**
Yes, the analyzer tracks salaries, infrastructure, marketing, legal, and office expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/burn-rate-analyzer](https://vinkius.com/mcp/burn-rate-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burn Rate Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `burn-rate-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burn Rate Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burn-rate-analyzer": {
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
