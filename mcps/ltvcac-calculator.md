# LTV:CAC Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ltvcac-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine if your customer acquisition strategy is profitable by calculating LTV, CAC, and the critical LTV:CAC ratio.

## Description
# Assess Unit Economics with Precision

The challenge for any growing business is knowing if spending money to acquire a customer actually generates profit. Many companies struggle to connect their marketing spend (CAC) directly to the long-term value of that customer (LTV). This gap in understanding leads to inefficient spending and unsustainable growth projections.

Our MCP provides a clear mechanism to bridge this financial intelligence gap. It guides users through three core calculations:

1. **Projecting Lifetime Value:** Using `calculate_ltv`, you input the Average Revenue Per User (ARPU), gross margin, and churn rate to forecast the total value of a customer over time.
2. **Pinpointing Acquisition Cost:** With `calculate_cac`, you provide detailed spend data across different channels. The tool computes the precise cost required to acquire one paying user from each source.
3. **Evaluating Profitability:** Finally, `evaluate_profitability` synthesizes these two metrics with your gross margin and time period to deliver the LTV:CAC ratio, a payback period in months, and a clear verdict (Optimal, Warning, or Critical).

The result is not just a number; it's an actionable measure of financial health. You can immediately determine if your marketing spend supports sustainable growth.


## Available Tools (3)
- **calculate_cac**: Accepts JSON array of {channelName, totalSpend, newCustomersAcquired} objects.

Calculate Customer Acquisition Cost (CAC) per marketing channel
- **calculate_ltv**: LTV = ARPU × (1 / churnRate) × grossMarginPercentage.

Calculate Customer Lifetime Value (LTV) based on ARPU, gross margin, and churn rate
- **evaluate_profitability**: Evaluate LTV:CAC ratio, payback period, and profitability verdict


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LTV:CAC Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My ARPU is $1200, gross margin is 0.65 (65%), and my annual churn rate is 0.08 (8%). Please calculate the LTV."

**🤖 AI Agent:**
> I will first run `calculate_ltv` with ARPU=1200, grossMarginPercentage=0.65, and churnRateAnnualPct=0.08. The projected LTV is $10,533.33.

---

**👤 You:**
> "Calculate CAC for these two channels: Paid Search ($20k spend, 40 customers) and Organic Content ($5k spend, 100 customers)."

**🤖 AI Agent:**
> Using `calculate_cac`, the resulting CAC is $0.50 for Paid Search ($20k/40) and $0.05 for Organic Content ($5k/100). Total CAC is $10,500.

---

**👤 You:**
> "Given an LTV of $10,533.33 and a total CAC of $10,500, with a gross margin of 0.65 over 12 months, what is the profitability verdict?"

**🤖 AI Agent:**
> I will run `evaluate_profitability` using LTV=$10533.33, totalCacAmount=$10500, grossMarginPercentage=0.65, and timePeriodMonths=12. The result shows an Optimal verdict (ratio > 5:1).


## ❓ FAQ

**Q: What is the most critical ratio to monitor?**
The LTV:CAC ratio is paramount. You can use `evaluate_profitability` by feeding it the results from `calculate_ltv` and `calculate_cac`. A healthy ratio (5:1 or higher) confirms that your acquisition spending generates sufficient long-term revenue.

**Q: How do I calculate LTV?**
Use the `calculate_ltv` tool. You must provide three inputs: ARPU, gross margin percentage (as a decimal), and the annual churn rate (also as a decimal). The resulting projected LTV is critical for subsequent steps.

**Q: Does this tool track CAC by channel?**
Yes. The `calculate_cac` tool accepts a JSON array of channel data, allowing you to calculate the specific Cost per Customer (CAC) for every source--be it paid search or social media.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltvcac-calculator](https://vinkius.com/mcp/ltvcac-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LTV:CAC Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ltvcac-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LTV:CAC Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ltvcac-calculator": {
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
