# Fill Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fill-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate Order, Line, and Unit Fill Rate metrics along with stockout costs.

## Description
This MCP server provides essential logistics performance tools to measure supply chain efficiency. Use `calculate_fill_rate_metrics` to determine Order, Line, and Unit Fill Rates from raw fulfillment data. The `estimate_stockout_impact` tool quantifies the financial loss and potential NPS degradation caused by unfulfilled orders. Additionally, `compare_to_benchmarks` allows you to evaluate your current performance against industry-specific targets for sectors like retail, pharmaceutical, electronics, and food & beverage.


## Available Tools
- **calculate_fill_rate_metrics**: Calculate Order, Line, and Unit Fill Rate metrics
- **compare_to_benchmarks**: Evaluate performance against industry benchmarks
- **estimate_stockout_impact**: Quantify the financial and reputational damage of unfulfilled demand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fill Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my fill rates for 100 total orders, 85 completed orders, 120 total lines, 100 completed lines, 500 units requested, and 450 units delivered."

**🤖 AI Agent:**
> The calculation results are: Order Fill Rate: 85.0%, Line Fill Rate: 83.3%, and Unit Fill Rate: 90.0%.

---

**👤 You:**
> "What is the financial impact of having 10 unfilled orders at a cost of $50 each with a high severity level?"

**🤖 AI Agent:**
> The total estimated stockout cost is $500, and the potential NPS impact is classified as 'high', indicating a significant risk of brand damage.

---

**👤 You:**
> "Compare my current unit fill rate of 85% against the pharmaceutical sector benchmark."

**🤖 AI Agent:**
> For the pharmaceutical sector, the benchmark is higher than your current 85%. Your performance status is 'Critical Failure'.


## ❓ FAQ

**Q: What is the difference between Order, Line, and Unit Fill Rate?**
Order Fill Rate tracks complete orders; Line Fill Rate measures accuracy at the SKU level; and Unit Fill Rate calculates the total volume of items delivered versus requested.

**Q: How can I estimate the cost of unfulfilled orders?**
Use the `estimate_stockout_impact` tool by providing the number of unfilled orders, the estimated cost per failed order, and the severity level of the service failure.

**Q: Does this tool support industry benchmarking?**
Yes, the `compare_to_benchmarks` tool compares your current unit fill rate against standard targets for sectors such as retail, pharmaceutical, electronics, and food & beverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fill-rate-calculator](https://vinkius.com/mcp/fill-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fill Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fill-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fill Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fill-rate-calculator": {
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
