# Food Delivery Fee Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-delivery-fee-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the true cost of Pickup, Delivery, and Dine-in options.

## Description
This MCP server provides a mathematical engine to calculate the total expenditure for food acquisition across different fulfillment models. It accounts for hidden costs like delivery markups, service fees, tips, and travel expenses. Use `compare_fulfillment_costs` to see a side-by-side comparison of Pickup, Delivery, and Dine-in, or `calculate_travel_impact` to see how distance affects your choice.


## Available Tools (4)
- **calculate_travel_impact**: Determines how physical distance shifts the economic favorability of Pickup vs. Delivery
- **compare_fulfillment_costs**: Compares the total cost of Pickup, Delivery, and Dine-in fulfillment models
- **get_delivery_fee_breakdown**: Isolates and displays the sum of all non-food costs associated with a delivery order
- **evaluate_markup_penalty**: Quantifies the financial penalty of using delivery services due to inflated menu prices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Delivery Fee Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the costs for a $50 order with a 15% delivery markup, a $5 delivery fee, a $3 service fee, a $5 tip, and a 10-mile distance with a $0.50 travel cost per mile."

**🤖 AI Agent:**
> The cheapest method is Pickup, costing $59.00, compared to Delivery at $78.25 and Dine-in at $55.00.

---

**👤 You:**
> "How much extra am I paying for delivery markup on a $30 order if the markup is 20%?"

**🤖 AI Agent:**
> The delivery markup penalty is $6.00, making the delivery base price $36.00.

---

**👤 You:**
> "What is the total of the delivery surcharges for a $4 fee, $2 service fee, and $6 tip?"

**🤖 AI Agent:**
> The total delivery surcharges are $12.00.


## ❓ FAQ

**Q: How does this tool calculate travel costs?**
Travel costs are calculated by multiplying the distance by the provided travel cost per unit. For Pickup, it calculates a round trip, while for Delivery, it calculates the one-way trip from the restaurant to your home.

**Q: What is a delivery markup?**
A delivery markup is the additional percentage added to the base menu price by third-party platforms. You can use `evaluate_markup_penalty` to see exactly how much this increases your total.

**Q: Can I compare specific delivery fees?**
Yes, you can use `get_delivery_fee_breakdown` to isolate and view the sum of delivery fees, service fees, and tips.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-delivery-fee-comparator](https://vinkius.com/en/ai-agent-connect/food-delivery-fee-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Delivery Fee Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-delivery-fee-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Delivery Fee Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-delivery-fee-comparator": {
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
