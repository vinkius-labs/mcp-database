# tea-leaf-cost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tea-leaf-cost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate tea costs for single servings, bulk batches, and inventory tiers.

## Description
This MCP server provides tools to manage and calculate tea-related costs. You can use `get_single_serving_cost` to find the price of a single cup, `calculate_bulk_batch_cost` for large production runs, `get_inventory_value_by_tier` to assess stock value by quality, and `compare_tea_affordability` to choose the most cost-effective tea option.


## Available Tools (4)
- **get_single_serving_cost**: Calculate the cost of a single serving of tea
- **calculate_bulk_batch_cost**: Calculate the cost of a large batch of tea
- **compare_tea_affordability**: Compare the cost-effectiveness of two tea options
- **get_inventory_value_by_tier**: Get the total value of tea inventory for a specific tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **tea-leaf-cost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does it cost to make a serving using 5 grams of tea at $0.50 per gram?"

**🤖 AI Agent:**
> The cost for a 5-gram serving is $2.50.

---

**👤 You:**
> "What is the cost of a batch of 1000 grams of tea at $0.20 per gram for 50 servings?"

**🤖 AI Agent:**
> The total batch cost is $200.00, which results in $4.00 per serving.

---

**👤 You:**
> "Which is cheaper for a 4g serving: Tea A at $0.60/g or Tea B at $0.50/g?"

**🤖 AI Agent:**
> Tea B is the cheaper option, with a price difference of $0.40 per serving.


## ❓ FAQ

**Q: How do I calculate the cost of one cup of tea?**
Use the `get_single_serving_cost` tool by providing the grams used and the price per gram.

**Q: Can I compare different tea brands?**
Yes, use `compare_tea_affordability` to determine which tea option is cheaper for a specific serving size.

**Q: How can I check my total stock value?**
You can use `get_inventory_value_by_tier` to see the total weight and monetary value of tea in specific quality tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tea-leaf-cost](https://vinkius.com/en/ai-agent-connect/tea-leaf-cost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **tea-leaf-cost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tea-leaf-cost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **tea-leaf-cost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tea-leaf-cost": {
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
