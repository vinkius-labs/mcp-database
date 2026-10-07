# Travel Luggage Fee Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-luggage-fee-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare airline baggage fees against shipping costs to find the cheapest travel strategy.

## Description
This MCP server provides a decision-support engine for travelers to optimize their luggage costs. By using tools like `compare_strategies`, you can evaluate whether it is more economical to pay airline baggage fees or to consolidate items into a single shipment via third-party logistics. The server handles complex calculations involving traveler counts, tiered airline pricing, and weight-based shipping quotes, ensuring you always choose the most cost-effective method for your trip.


## Available Tools (4)
- **get_shipping_quote**: Get a shipping quote for a total weight
- **validate_bag_weight**: Validate if a bag weight is within airline limits
- **calculate_airline_fees**: Calculate total airline fees for a set of bags
- **compare_strategies**: Compare airline baggage strategies against shipping options


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Luggage Fee Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare baggage strategies for 2 travelers. Plan A: two 20kg bags. Plan B: one 40kg shipment. Shipping options: Standard at $50."

**🤖 AI Agent:**
> The cheapest strategy is shipping, with a total cost of $50, saving you money compared to airline fees.

---

**👤 You:**
> "Is a 35kg bag allowed on Airline_Alpha?"

**🤖 AI Agent:**
> No, the bag exceeds the maximum allowed weight of 32kg for Airline_Alpha by 3kg.

---

**👤 You:**
> "Get a shipping quote for 15kg using express service."

**🤖 AI Agent:**
> The express shipping quote for 15kg is $75 with an estimated delivery of 3 days.


## ❓ FAQ

**Q: How does the tool calculate airline costs?**
The `calculate_airline_fees` tool sums the fees for every bag in your plan and multiplies that total by the number of travelers to get the full trip cost.

**Q: Can I check if my bag is too heavy for a specific airline?**
Yes, you can use `validate_bag_weight` to check if a specific weight exceeds the limits set by a chosen airline.

**Q: Does this tool consider shipping costs?**
Yes, the `compare_strategies` tool evaluates both airline baggage fees and shipping quotes to recommend the cheapest option.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-luggage-fee-comparator](https://vinkius.com/en/ai-agent-connect/travel-luggage-fee-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Luggage Fee Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-luggage-fee-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Luggage Fee Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-luggage-fee-comparator": {
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
