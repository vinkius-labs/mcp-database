# Growth Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/growth-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate MoM, QoQ, YoY growth rates and model multi-scenario financial projections (CAGR, Rule of 40) from historical revenue data.

## Description
# Assess Growth Trajectory with Financial Precision

The core challenge for any growing business is quantifying performance over time. Simply looking at last month's revenue is insufficient; true financial health requires comparing current results against historical benchmarks (like the same quarter last year) and projecting future potential under different growth assumptions.

This MCP provides a systematic way to analyze sequential financial data, moving beyond simple arithmetic averages to provide actionable metrics: directional momentum (MoM/QoQ), long-term stability (YoY/CAGR), and operational efficiency (Rule of 40).

## How the System Works (The Mechanism)

The server operates through three connected tools that model different aspects of financial performance:

1. **Analyzing Directional Momentum:** Use `analyze_historical_growth` to instantly calculate Month-over-Month, Quarter-over-Quarter, and Year-over-Year growth rates across your entire dataset. This identifies immediate trends and volatility.
2. **Synthesizing Core Benchmarks:** Next, run `calculate_key_rates`. By feeding the historical revenue and EBITDA data, this tool computes two critical benchmarks: the Compound Annual Growth Rate (CAGR) for overall sustained growth, and the Rule of 40 score, which combines your growth rate with profitability.
3. **Forecasting Future Potential:** Finally, use `generate_growth_projection`. This tool takes the most recent revenue figure and projects a full twelve months into the future, allowing you to model 'Constant', 'Accelerated', or 'Decelerated' scenarios based on your expected market shifts.

The result is not just a set of numbers; it is a comprehensive financial blueprint that helps determine if your growth rates are sustainable, profitable, and where your business stands relative to key industry benchmarks.


## Available Tools (3)
- **analyze_historical_growth**: Pass data as a JSON array of objects with date and revenue fields.

Analyze historical revenue growth across time periods
- **calculate_key_rates**: Pass EBITDA metrics as a JSON array of {revenue, ebitda} objects.

Calculate CAGR and Rule of 40 score from financial data
- **generate_growth_projection**: For Accelerated/Decelerated, provide rateDeterminer as the monthly rate shift percentage.

Generate 12-month revenue projections under different growth scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Growth Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have historical revenue data for the last 3 years, and I want to see my MoM, QoQ, and YoY growth rates. The data includes dates from '2021-01' to '2023-12'."

**🤖 AI Agent:**
> Run the `analyze_historical_growth` tool with my data points and set the time granularity to 'Month'. This will show me all directional changes.

---

**👤 You:**
> "Based on my 5 years of revenue data and associated EBITDA, what is my CAGR and Rule of 40 score?"

**🤖 AI Agent:**
> I need to use the `calculate_key_rates` tool. I will provide the start value, end value, years elapsed (5), and a list of all historical revenue/EBITDA metrics for accurate calculation.

---

**👤 You:**
> "Project my revenue for the next year assuming aggressive, accelerating growth. My last known revenue was $10M, and I estimate a monthly rate shift of +7%."

**🤖 AI Agent:**
> I will use the `generate_growth_projection` tool. I'll set the last known revenue to 10,000,000, the horizon months to 12, the scenario to 'Accelerated', and provide the base monthly growth rate (if applicable) and the rate determiner of 7%.


## ❓ FAQ

**Q: Does the calculator only look at monthly data?**
No. The `analyze_historical_growth` tool allows you to specify the time granularity ('Month', 'Quarter', or 'Year'). This ensures that whether you are looking for short-term momentum (MoM) or long-term seasonal trends (YoY), the comparison is accurate based on your data.

**Q: What is the difference between CAGR and Rule of 40?**
CAGR measures the overall smooth, annualized growth rate over a long period. The Rule of 40 uses `calculate_key_rates` to provide a composite score (Growth Rate % + EBITDA Margin %). It is a single metric that tells investors about both revenue expansion and operational profitability simultaneously.

**Q: Can I predict revenue for more than 12 months?**
The `generate_growth_projection` tool is designed to project a full twelve-month (12-month) forecast horizon. While you can adjust the inputs, the default and most reliable projection window provided by this server is exactly one year.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growth-rate-calculator](https://vinkius.com/mcp/growth-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Growth Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `growth-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Growth Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "growth-rate-calculator": {
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
