# Campaign ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/campaign-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate net profit, ROI, and break-even points for marketing campaigns.

## Description
This MCP server provides essential financial analysis tools for marketing professionals. It connects AI agents to precise profitability calculations, allowing for deep analysis of campaign performance. Use `get_campaign_profitability` to determine net profit and ROI, `get_efficiency_metrics` to analyze lead costs, `get_break_even_analysis` to find profitability thresholds, and `get_scenario_projection` to simulate scaling budgets or improving conversion rates.


## Available Tools (4)
- **get_campaign_profitability**: Calculate the actual net profit and ROI for a specific campaign
- **get_efficiency_metrics**: Calculate cost per lead and revenue per conversion
- **get_scenario_projection**: Project profit and ROI for scaled spend or improved conversion
- **get_break_even_analysis**: Determine required leads or conversion rate to reach break-even


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campaign ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the actual net profit and ROI for a campaign with $5000 spend, 1000 leads, 5% conversion, $100 AOV, 2% refund rate, and $10 fulfillment cost?"

**🤖 AI Agent:**
> The total revenue was $5,000.00, the net profit was $3,910.00, and the ROI was 0.782.

---

**👤 You:**
> "How much does each lead cost for a campaign with $2000 spend and 500 leads?"

**🤖 AI Agent:**
> The cost per lead is $4.00.

---

**👤 You:**
> "What happens to my profit if I double my $1000 spend and increase conversion from 2% to 4%? (Current: 1000 leads, $50 AOV, 1% refund, $5 fulfillment)"

**🤖 AI Agent:**
> By doubling the spend and improving conversion, your projected net profit is $156.00 with a projected ROI of 0.156.


## ❓ FAQ

**Q: How do I calculate my campaign's net profit?**
You can use the `get_campaign_profitability` tool by providing your ad spend, lead count, conversion rate, average order value, refund rate, and fulfillment cost per order.

**Q: Can I simulate what happens if I double my budget?**
Yes, use the `get_scenario_projection` tool and set the scaling factor to 2.0 to see the projected impact on profit and ROI.

**Q: How do I find out when my campaign will become profitable?**
The `get_break_even_analysis` tool calculates the required leads or conversion rate needed to reach a zero-profit threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/campaign-roi-calculator](https://vinkius.com/en/ai-agent-connect/campaign-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campaign ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `campaign-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campaign ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campaign-roi-calculator": {
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
