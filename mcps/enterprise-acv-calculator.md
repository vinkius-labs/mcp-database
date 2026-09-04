# Enterprise ACV Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-acv-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Annual Contract Value, segment metrics, and discount impact.

## Description
This MCP server provides precise financial tools for analyzing contract value. Use `get_acv_summary` to calculate the annualized value of a single contract, including expansions and discounts. Use `get_segment_metrics` to aggregate data across customer segments, or `analyze_discount_impact` to evaluate revenue loss from discounts. For multi-year deals with scheduled increases, `get_ramped_acv_projection` provides yearly revenue forecasts.


## Available Tools (4)
- **analyze_discount_impact**: Evaluates the financial effect of discounts on the total contract value and the annualized value
- **get_acv_summary**: Calculates the primary annualized value of a single contract
- **get_ramped_acv_projection**: Predicts the specific revenue expected in each year of a contract with a ramp period
- **get_segment_metrics**: Aggregates ACV data to provide insights into different customer segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise ACV Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ACV for a $120,000 contract with a 12-month term and a 10% discount?"

**🤖 AI Agent:**
> The ACV for this contract is $108,000.

---

**👤 You:**
> "Calculate the average ACV for these contracts: [{ "acv": 50000, "segment": "Enterprise" }, { "acv": 30000, "segment": "Enterprise" }]"

**🤖 AI Agent:**
> The average ACV for the Enterprise segment is $40,000.

---

**👤 You:**
> "Show me the yearly revenue projection for a $100,000 contract over 3 years with increases of $5,000 and $10,000 each year."

**🤖 AI Agent:**
> Year 1: $100,000, Year 2: $105,000, Year 3: $115,000. Total value: $320,000.


## ❓ FAQ

**Q: How is ACV calculated?**
ACV is calculated by taking the total net contract value (base value plus expansions, minus discounts) and dividing it by the total number of years in the term.

**Q: Can I analyze revenue loss from discounts?**
Yes, you can use the `analyze_discount_impact` tool to see the total and annual revenue lost due to applied discounts.

**Q: Does this support multi-year contracts with ramp periods?**
Yes, the `get_ramped_acv_projection` tool allows you to project specific revenue for each year based on scheduled increases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-acv-calculator](https://vinkius.com/ai-agent-connect/enterprise-acv-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise ACV Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-acv-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise ACV Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-acv-calculator": {
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
