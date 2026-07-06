# LTV Cohort Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ltv-cohort-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate Customer Lifetime Value (LTV) for any acquisition cohort, projecting future revenue trends.

## Description
**[Hook]** Understanding the true value of a customer group is critical to sustainable business growth. But raw revenue data doesn't tell the full story.


## Available Tools (3)
- **generate_ltv_projections**: Historical metrics must be provided as a JSON array of objects with periodIndex and accumulatedRevenueValue fields.

Project LTV at 36 months using linear and logarithmic extrapolation methods
- **calculate_cumulative_ltv**: Milestones are specified as months after acquisition.

Calculate total accumulated LTV at fixed milestones for a cohort
- **fetch_cohort_metrics**: Use acquireMonth in YYYY-MM format and optionally specify how many months of history to retrieve.

Fetch raw accumulated monthly revenues for a given acquisition cohort


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LTV Cohort Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Please analyze the '2023-01' cohort. First, fetch all historical revenue data for 36 months, and then calculate its LTV at 3, 6, and 12 months."

**🤖 AI Agent:**
> First, I will call `fetch_cohort_metrics(acquireMonth='2023-01', cohortLengthMonths=36)` to get the full revenue history. Then, using that data, I will run `calculate_cumulative_ltv(cohortIdentifier='2023-01', targetMilestones=[3, 6, 12])`.

---

**👤 You:**
> "I need a long-term forecast for the '2022-11' cohort. Project its LTV to 36 months using both linear and logarithmic methods."

**🤖 AI Agent:**
> To project the LTV, I must first compile the historical data by calling `fetch_cohort_metrics(acquireMonth='2022-11', cohortLengthMonths=36)`. Once I have the full metrics JSON array, I will pass it to `generate_ltv_projections` for the final forecast.

---

**👤 You:**
> "What is the current LTV status of the '2023-04' cohort at 24 months?"

**🤖 AI Agent:**
> I will use the `calculate_cumulative_ltv` tool, specifying `cohortIdentifier='2023-04'` and `targetMilestones=[24]`. This provides the accurate cumulative LTV up to the 24-month mark.


## ❓ FAQ

**Q: How do I get the raw historical revenue data needed for LTV calculations?**
Use the `fetch_cohort_metrics` tool. This function retrieves the accumulated monthly revenues for a specific cohort, providing the foundational time-series data required for all subsequent LTV analyses.

**Q: What is the difference between calculating LTV at fixed milestones (e.g., 6 months) and projecting future value?**
First, use `calculate_cumulative_ltv` to determine the exact LTV at fixed points (like 3 or 6 months). Then, if you need a longer-term forecast, feed those historical metrics into `generate_ltv_projections`. The projection tool uses advanced math to estimate value beyond observed data.

**Q: What inputs are required for LTV projections?**
The `generate_ltv_projections` tool requires two key pieces of information: the unique cohort identifier and a structured JSON array containing historical revenue metrics. This data is typically sourced from running `fetch_cohort_metrics` first.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltv-cohort-calculator](https://vinkius.com/mcp/ltv-cohort-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LTV Cohort Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ltv-cohort-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LTV Cohort Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ltv-cohort-calculator": {
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
