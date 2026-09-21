# Subscription Box Unit Economics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subscription-box-unit-economics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate profitability, LTV, and payback periods for subscription box models.

## Description
This MCP server provides a complete financial modeling engine for subscription box businesses. It allows AI agents to calculate core profitability metrics including contribution margin, customer lifetime value (LTV), and payback periods. Users can perform detailed cost analysis using `get_margin_breakdown` to identify cost-heavy areas, run sensitivity tests with `analyze_sensitivity` to see how cost changes impact LTV, and project long-term profitability using `simulate_cohort_growth`. The engine handles complex variables like shipping costs, payment fees, and churn rates to provide accurate economic insights.


## Available Tools (4)
- **analyze_sensitivity**: Evaluates how much the LTV changes when a specific cost or rate is adjusted
- **calculate_unit_economics**: Calculates fundamental profitability metrics (Contribution Margin and LTV) for a single subscription unit
- **get_margin_breakdown**: Provides a detailed view of where the revenue is going to identify cost-heavy areas
- **simulate_cohort_growth**: Projects the total monthly profit of a cohort over time based on initial acquisition and churn


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Box Unit Economics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the unit economics for a box priced at $40 with a $15 product cost, $5 packaging, $3 fulfillment, $6 shipping, a 3% payment fee, and 5% monthly churn."

**🤖 AI Agent:**
> The contribution margin is $14.88, the LTV is $297.60, the payback period is 3.4 months, and the break-even churn rate is 37.2%.

---

**👤 You:**
> "Show me the cost breakdown for a $50 subscription box where product costs are $20 and shipping is $8."

**🤖 AI Agent:**
> The total variable costs are $32.50, leaving a net margin of $17.50. Product costs account for 40% of the price, while shipping accounts for 16%.

---

**👤 You:**
> "If I increase my product cost by $2, how much will my LTV decrease?"

**🤖 AI Agent:**
> Increasing the product cost by $2 reduces the LTV from $300.00 to $240.00, representing a 20% decrease.


## ❓ FAQ

**Q: How does this tool calculate LTV?**
LTV is calculated by dividing the contribution margin per unit by the monthly churn rate.

**Q: Can I test how shipping increases affect my profit?**
Yes, you can use the `analyze_sensitivity` tool to adjust the shipping cost and see the resulting change in LTV.

**Q: What is included in the contribution margin?**
The contribution margin is the effective price (monthly price minus discounts) minus all variable costs: product, packaging, fulfillment, shipping, and payment fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subscription-box-unit-economics-engine](https://vinkius.com/en/ai-agent-connect/subscription-box-unit-economics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Box Unit Economics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-box-unit-economics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Box Unit Economics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-box-unit-economics-engine": {
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
