# Service Pricing Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/service-pricing-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate precise service quotes by calculating labor, travel, materials, overhead, and profit.

## Description
This MCP server provides a specialized engine for generating accurate service quotes. It integrates multiple cost pillars including direct costs (labor, travel, materials, and revisions), service adjustments (overhead), and profitability targets (profit and tax). Use `calculate_quote` to generate a full itemized quote, `estimate_overhead_impact` to see how overhead affects direct costs, `analyze_profit_margins` to evaluate margin and markup, and `validate_quote_feasibility` to ensure a proposed price meets minimum profit requirements after taxes.


## Available Tools (4)
- **analyze_profit_margins**: Evaluates the relationship between the target profit and the total cost to understand the project's margin profile
- **calculate_quote**: Generates a complete, itemized service quote based on all provided cost and margin variables
- **estimate_overhead_impact**: Determines how much overhead will be added to a quote given specific direct costs and a rate
- **validate_quote_feasibility**: Checks if a proposed quote meets minimum business requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Service Pricing Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a quote with $500 labor, $100 travel, $200 materials, 10% overhead, $300 profit, and 5% tax."

**🤖 AI Agent:**
> The final quote is $1,215.00.

---

**👤 You:**
> "What is the markup percentage if my total cost is $1000 and my target profit is $250?"

**🤖 AI Agent:**
> The markup percentage is 25%.

---

**👤 You:**
> "Will a $1500 quote be feasible if I need at least $200 profit and the tax rate is 8%?"

**🤖 AI Agent:**
> Yes, the quote is feasible with a remaining margin of $1,380.00 above the minimum profit.


## ❓ FAQ

**Q: How does the tool calculate the final quote?**
The `calculate_quote` tool sums the direct costs (labor, travel, materials, and revisions), adds the overhead amount calculated from the overhead rate, and then adds the tax amount calculated from the total cost.

**Q: Can I check if my profit margin is sufficient?**
Yes, you can use `analyze_profit_margins` to see your profit margin percentage and markup percentage, or `validate_quote_feasibility` to check if a specific quote meets your minimum profit needs.

**Q: What is included in the direct costs?**
Direct costs consist of labor, travel, materials, and any planned revisions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/service-pricing-builder](https://vinkius.com/en/ai-agent-connect/service-pricing-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Service Pricing Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `service-pricing-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Service Pricing Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "service-pricing-builder": {
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
