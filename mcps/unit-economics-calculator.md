# Unit Economics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unit-economics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine if your customer acquisition strategy is profitable by calculating LTV, CAC, and the critical LTV:CAC ratio using three interconnected financial models.

## Description
# Assess Unit Economics with Precision

The challenge for any growing business is knowing if spending money to acquire a customer actually generates profit. Many companies struggle to connect their marketing spend (CAC) directly to the long-term value of that customer (LTV). This gap in understanding leads to inefficient spending and unsustainable growth projections.

Our MCP provides a clear mechanism to bridge this financial intelligence gap by running three sequential, interconnected calculations:

1. **Calculate Initial Profitability:** Start with `calculate_contribution_margin`. You input the Gross Price, COGS per Customer, and Support Cost per Customer to determine the immediate profit generated in one billing cycle.
2. **Estimate Lifetime Value (LTV):** Next, use `calculate_payback_period`'s underlying logic (or a dedicated LTV estimation tool) by feeding the monthly contribution margin and the expected Churn Rate into the model to project the total potential revenue over time.
3. **Determine Payback & Net Value:** Finally, run `calculate_payback_period`. This step takes the projected LTV and the amortized CAC to give you two critical numbers: the exact number of months required to recover your acquisition cost, and the resulting net residual margin--the true measure of sustainable profitability.

The result is not just a number; it's an actionable blueprint for financial health. You can immediately determine if your marketing spend supports profitable growth by systematically modeling unit economics from initial margins to long-term viability.


## Available Tools
- **calculate_contribution_margin**: Calculate contribution margin from revenue and variable costs
- **rate_health**: Rate unit economics health based on payback period
- **calculate_payback_period**: Calculate customer acquisition cost payback period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unit Economics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The gross price is $100, COGS is $30, and support costs $5. The CAC is $400. Estimate the payback period."

**🤖 AI Agent:**
> First, I'll call `calculate_contribution_margin` with (100, 30, 5) to get a monthly margin of $65. Then, I will use `calculate_payback_period` with CAC=$400 and Margin=$65. The payback period is approximately 7 months.

---

**👤 You:**
> "I need to know if a $2,000 CAC is viable given a monthly margin of $150 and an estimated LTV of $3,000."

**🤖 AI Agent:**
> Running the numbers through `calculate_payback_period` shows that with a $150 margin, recovering a $2,000 CAC requires about 14 months. This is crucial for assessing long-term viability.

---

**👤 You:**
> "What if my COGS increases to $45? Calculate the new unit margin and rate the health."

**🤖 AI Agent:**
> I will first use `calculate_contribution_margin` (Revenue, $100; Costs, $45 + $5) to get a lower margin. Then, using that new margin, I can evaluate the unit economics health with `rate_health`.


## ❓ FAQ

**Q: What is the first step to calculating profitability?**
You must first use `calculate_contribution_margin` by providing the Gross Price, COGS, and Support Cost. This establishes the core monthly profit before considering long-term effects.

**Q: How do I find out if my CAC is sustainable?**
Use `calculate_payback_period`. This tool takes your Customer Acquisition Cost and the monthly contribution margin to tell you exactly how many months it will take to break even. A lower number means better unit economics.

**Q: What is the final measure of long-term value?**
The most comprehensive view comes from `calculate_payback_period`. It synthesizes all inputs to provide a Net LTV Residual Margin, which is the true profit left over after paying back your CAC and accounting for churn.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unit-economics-calculator](https://vinkius.com/mcp/unit-economics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unit Economics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unit-economics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unit Economics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unit-economics-calculator": {
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
