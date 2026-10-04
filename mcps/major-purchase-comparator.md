# Major Purchase Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/major-purchase-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Rank products using weighted metrics like price, running cost, and warranty.

## Description
This MCP server provides decision-support tools to identify the optimal purchase by calculating weighted scores for competing products. It evaluates items through multiple lenses including purchase price, running cost, delivery speed, warranty duration, feature sets, and user ratings. Use `compare_products` to rank a group of items, `calculate_tco` to find the total cost of ownership, `validate_weight_configuration` to ensure your priorities are balanced, or `summarize_product_profiles` to see high-level highlights like the cheapest or most feature-rich option.


## Available Tools (4)
- **compare_products**: Performs the core mathematical ranking of multiple products based on user-defined weights and product attributes
- **summarize_product_profiles**: Provides a high-level comparison of the diversity of the product group
- **validate_weight_configuration**: Ensures that the user's prioritization strategy is mathematically sound and balanced
- **calculate_tco**: Determines the total cost of ownership for a single product over a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Major Purchase Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these three laptops: Laptop A ($1000, 2yr warranty, 5 features, 4.5 rating), Laptop B ($1200, 3yr warranty, 7 features, 4.2 rating), and Laptop C ($900, 1yr warranty, 4 features, 4.0 rating). Weight price and warranty heavily."

**🤖 AI Agent:**
> Laptop B is the winner with a total score of 85, followed by Laptop A with 78 and Laptop C with 62.

---

**👤 You:**
> "What is the total cost of ownership for a vacuum costing $300 with an annual running cost of $50 over 5 years?"

**🤖 AI Agent:**
> The total cost of ownership is $550.

---

**👤 You:**
> "Summarize these products: Product X ($50, 4 rating, 2yr warranty), Product Y ($80, 5 rating, 3yr warranty), Product Z ($40, 3 rating, 1yr warranty)."

**🤖 AI Agent:**
> The cheapest product is Product Z, the best rated is Product Y, the longest warranty is Product Y, and the most feature rich is Product X.


## ❓ FAQ

**Q: How does the ranking work?**
The system normalizes each attribute against the best performer in its category and applies your assigned weights. For costs, lower values score higher; for features and ratings, higher values score higher.

**Q: What is Total Cost of Ownership (TCO)?**
TCO is the sum of the initial purchase price and the accumulated running costs over the expected lifecycle of the product.

**Q: Can I use this to compare appliances?**
Yes, it is ideal for any major purchase where you need to balance upfront costs against long-term running costs and features.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/major-purchase-comparator](https://vinkius.com/en/ai-agent-connect/major-purchase-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Major Purchase Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `major-purchase-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Major Purchase Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "major-purchase-comparator": {
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
