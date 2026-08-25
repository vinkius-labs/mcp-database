# Accelerator Portfolio Markup Frequency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-portfolio-markup-frequency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze valuation velocity and magnitude for portfolio companies and aggregate metrics.

## Description
This MCP server provides tools to analyze the velocity and magnitude of valuation adjustments within an accelerator's investment portfolio. It connects AI agents to critical venture capital metrics, allowing for deep analysis of company-specific markup frequency and overall portfolio health. Use `analyze_company_markup_velocity` to track how often a specific company's value changes, `calculate_portfolio_markup_metrics` to assess aggregate momentum and volatility, or `project_value_trend` to visualize the trajectory of total portfolio value over time.


## Available Tools (3)
- **analyze_company_markup_velocity**: Analyzes the frequency and magnitude of valuation changes for a specific company
- **calculate_portfolio_markup_metrics**: Calculates aggregate health and valuation momentum for the entire portfolio
- **project_value_trend**: Projects the trajectory of the portfolio value over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Portfolio Markup Frequency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How frequently and by how much has company ABC changed in value?"

**🤖 AI Agent:**
> Company ABC has an average valuation change frequency of 14 months, with an average magnitude of 22% per event.

---

**👤 You:**
> "What is the overall health of my portfolio over the last 12 months?"

**🤖 AI Agent:**
> The portfolio shows an aggregate markup rate of 15.4% with a total portfolio value of $45,000,000 over the last 12 months.

---

**👤 You:**
> "Show me the trend of my portfolio value on a quarterly basis."

**🤖 AI Agent:**
> The portfolio value has grown from $38M in Q1 to $45M in Q4, showing a steady upward trajectory.


## ❓ FAQ

**Q: How is markup frequency calculated?**
Frequency is determined by calculating the time elapsed between consecutive valuation events, such as funding rounds or 409A appraisals.

**Q: Can I filter valuation types for a specific company?**
Yes, by using `analyze_company_markup_velocity`, you can provide an array of valuation types like 'funding_round' or '409a' to filter the results.

**Q: What does the portfolio volatility metric represent?**
Portfolio volatility is derived from the variance in magnitude across all valuation events within the specified timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-portfolio-markup-frequency](https://vinkius.com/ai-agent-connect/accelerator-portfolio-markup-frequency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Portfolio Markup Frequency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-portfolio-markup-frequency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Portfolio Markup Frequency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-portfolio-markup-frequency": {
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
