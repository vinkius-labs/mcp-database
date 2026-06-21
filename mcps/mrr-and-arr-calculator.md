# MRR and ARR Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mrr-and-arr-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Monthly Recurring Revenue (MRR) and Annual Recurring Revenue (ARR) from subscription data, broken down by plan segment.

## Description
Building a financial forecast requires more than just total revenue. The challenge is accurately separating the source of growth: where did the money come from? Was it new customers, existing customer upgrades, or was it lost to cancellations?

The MRR and ARR Calculator solves this by providing granular tracking for every component of recurring revenue--New, Expansion, and Churn. It connects raw subscription data (plan price, unit count) to actionable financial metrics.

**Mechanism:** The system uses specialized tools to process your time-series data. First, the `calculate_mrr` tool processes a batch of subscriptions to yield the total MRR for a period. This result is then passed to `aggregate_mrr_components` to separate New, Expansion, and Churn revenue streams. Finally, the `calculate_arr` and `get_metrics_summary` tools take these core metrics to provide annualized forecasts (ARR) and key ratios like ARPU.

**Advantage:** Instead of a single gross number, you get a full financial picture: how fast are you growing (Net New MRR), and what is the true value of your customer base? This allows for precise forecasting and strategic decision-making.


## Available Tools
- **calculate_arr**: Calculate Annual Recurring Revenue from MRR
- **calculate_churn_impact**: Calculate the impact of customer churn on revenue
- **get_metrics_summary**: Get a comprehensive SaaS metrics summary
- **calculate_mrr**: Calculate Monthly Recurring Revenue from subscription data
- **project_revenue**: Project revenue for a given time period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MRR and ARR Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have subscription data for January: 100 seats @ $5/seat, and 20 new seats added. Calculate the total MRR."

**🤖 AI Agent:**
> Use `calculate_mrr` with the subscription data. This will output a total MRR figure, which you can then use to calculate the ARR using `calculate_arr`.

---

**👤 You:**
> "I want to see my projected revenue for the next 12 months, starting from a current MRR of $50,000."

**🤖 AI Agent:**
> Run `project_revenue` with an MRR of 50000 and months set to 12. This provides the annualized forecast you requested.

---

**👤 You:**
> "My MRR was $80,000 last month, and my current churn rate is 5%. What does that mean for my next period?"

**🤖 AI Agent:**
> Use the `calculate_churn_impact` tool. Input your $80,000 MRR and 5% churn rate to understand the potential revenue loss.


## ❓ FAQ

**Q: What is the difference between MRR and ARR?**
MRR tracks predictable monthly revenue. To annualize this, use the `calculate_arr` tool. It takes your calculated MRR figure and multiplies it by twelve to give you the Annual Recurring Revenue (ARR).

**Q: How do I separate New, Expansion, and Churn revenue?**
You must first use the `calculate_mrr` tool to get the total MRR. Then, pass this detailed output into a subsequent aggregation step (conceptually represented by `aggregate_mrr_components`) to get the breakdown of New, Expansion, and Churn revenue streams.

**Q: Can I project future revenue based on current growth?**
Yes. After calculating your Net New MRR, you can use the `project_revenue` tool. This tool takes a starting MRR and the number of months (1-36) to generate a projected revenue total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mrr-and-arr-calculator](https://vinkius.com/mcp/mrr-and-arr-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MRR and ARR Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mrr-and-arr-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MRR and ARR Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mrr-and-arr-calculator": {
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
