# Museum Ticket Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/museum-ticket-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total museum ticket costs for groups and individuals.

## Description
This MCP server provides tools to manage museum ticket pricing. You can use `get_category_prices` to see current rates, `calculate_individual_price` for single visitors, and `calculate_group_total` to find the sum for entire groups, including potential volume discounts. It also includes `validate_visitor_data` to ensure input counts are correct.


## Available Tools (4)
- **validate_visitor_data**: Ensures that the provided visitor information is logically sound
- **calculate_group_total**: Calculates the total cost for a specific group of visitors
- **calculate_individual_price**: Determines the cost of a single ticket based on the visitor profile
- **get_category_prices**: Retrieves the current standard ticket prices for each visitor category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Museum Ticket Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the ticket prices in the USA?"

**🤖 AI Agent:**
> In the USA, the prices are: Adult: $25, Child: $15, Senior: $20.

---

**👤 You:**
> "How much will it cost for 2 adults and 1 child in Europe?"

**🤖 AI Agent:**
> The total cost for 2 adults and 1 child in Europe is €65.

---

**👤 You:**
> "Calculate the total for a group of 10 adults in the USA with a group discount."

**🤖 AI Agent:**
> The total cost for 10 adults in the USA with the group discount applied is $200.


## ❓ FAQ

**Q: How do I check the prices for different regions?**
You can use the `get_category_prices` tool and specify the region, such as 'USA' or 'Europe'.

**Q: Can I apply a group discount?**
Yes, when using `calculate_group_total`, you can set the `applyGroupDiscount` parameter to true to check if the group meets the required headcount threshold.

**Q: Does membership affect the price?**
Yes, using `calculate_individual_price` with the `hasMembership` flag set to true will apply the membership discount to the base price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/museum-ticket-calculator](https://vinkius.com/en/ai-agent-connect/museum-ticket-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Museum Ticket Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `museum-ticket-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Museum Ticket Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "museum-ticket-calculator": {
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
