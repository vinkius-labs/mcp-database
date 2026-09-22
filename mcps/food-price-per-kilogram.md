# Food Price per Kilogram MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-price-per-kilogram)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and compare food unit prices per kilogram to find the best value.

## Description
This MCP server provides tools to normalize food costs by calculating the price per kilogram. It allows you to convert different weight units, compare the value between two different packages, and determine if buying in bulk offers significant savings. Use `calculate_unit_price` to find the cost of a single kilogram, `compare_unit_prices` to see which item is cheaper, `convert_weight_to_kg` for mass normalization, and `get_bulk_savings_threshold` to analyze bulk deals.


## Available Tools (4)
- **calculate_unit_price**: Calculate the price per kilogram for a food item
- **compare_unit_prices**: Compare the unit price of two food items
- **convert_weight_to_kg**: Convert a given weight to kilograms
- **get_bulk_savings_threshold**: Determine if a bulk package offers significant savings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Price per Kilogram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does a 500g bag of flour costing $2.50 cost per kilogram?"

**🤖 AI Agent:**
> $5.00 per kilogram.

---

**👤 You:**
> "Which is a better deal: 1kg of rice for $3.00 or 500g of rice for $1.60?"

**🤖 AI Agent:**
> The 1kg bag for $3.00 is the better deal.

---

**👤 You:**
> "Convert 250 grams to kilograms."

**🤖 AI Agent:**
> 0.25 kg


## ❓ FAQ

**Q: How do I calculate the price per kilogram?**
You can use the `calculate_unit_price` tool by providing the total package cost, the weight, and the unit (kg or g).

**Q: Can I compare two different brands?**
Yes, use the `compare_unit_prices` tool to determine which package offers the better value per kilogram.

**Q: Does it support grams?**
Yes, the tools support weight normalization for grams (g), kilograms (kg), and milligrams (mg).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-price-per-kilogram](https://vinkius.com/en/ai-agent-connect/food-price-per-kilogram)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Price per Kilogram** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-price-per-kilogram` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Price per Kilogram** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-price-per-kilogram": {
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
