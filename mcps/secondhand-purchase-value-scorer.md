# Secondhand Purchase Value Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/secondhand-purchase-value-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the true value of used items by comparing them to brand-new prices.

## Description
This MCP server provides tools to calculate the economic value of secondhand items. By analyzing listing prices, condition scores, expected remaining life, and potential repair costs against a new-item reference price, it helps users identify the best deals. Use `calculate_item_value` to score a single item, `rank_multiple_listings` to sort a list of options, `get_repair_impact_analysis` to see how repairs affect value, or `compare_two_items` for head-to-head comparisons.


## Available Tools (4)
- **compare_two_items**: Provides a direct head-to-head comparison between two different used item listings
- **calculate_item_value**: Calculates a single value score for a specific used item
- **get_repair_impact_analysis**: Evaluates how much a specific repair cost diminishes the value
- **rank_multiple_listings**: Ranks a collection of different used item listings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Secondhand Purchase Value Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the value of a used laptop listed at $400, with a new price of $1000, a condition score of 0.8, 3 years of life remaining, $50 repair cost, and $20 delivery cost. Use equal weights for all factors."

**🤖 AI Agent:**
> The calculated value score for this laptop is 0.72, with a savings ratio of 0.57.

---

**👤 You:**
> "Compare two used bikes. Bike A: $200, new price $500, condition 0.9, 5 years life, $0 repair, $10 delivery. Bike B: $150, new price $500, condition 0.6, 2 years life, $40 repair, $5 delivery. Use weights: price 0.4, condition 0.3, life 0.2, repair 0.1."

**🤖 AI Agent:**
> Bike A is the better deal with a higher value score.

---

**👤 You:**
> "How much will a $100 repair cost reduce the value of a used camera priced at $300 (new price $800, condition 0.8, 4 years life, $0 delivery, weights: price 0.3, condition 0.3, life 0.2, repair 0.2)?"

**🤖 AI Agent:**
> The repair will cause a 12% drop in the item's value score.


## ❓ FAQ

**Q: How is the value score calculated?**
The score is calculated by applying user-defined weights to the item's condition, expected life, price, and repair costs, relative to the cost of buying the item brand new.

**Q: Can I prioritize certain factors like condition over price?**
Yes, you can use `userWeights` to specify how much importance to give to condition, life, price, and repair costs.

**Q: How do I compare multiple used items at once?**
You can use the `rank_multiple_listings` tool to provide a list of items and receive a ranked list from highest to lowest value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/secondhand-purchase-value-scorer](https://vinkius.com/en/ai-agent-connect/secondhand-purchase-value-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Secondhand Purchase Value Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `secondhand-purchase-value-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Secondhand Purchase Value Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "secondhand-purchase-value-scorer": {
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
