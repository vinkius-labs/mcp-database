# Wholesale Order Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wholesale-order-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate wholesale order totals, tiered pricing, and eligibility.

## Description
This MCP server provides precision calculation tools for wholesale operations. It allows AI agents to determine exact order totals using `calculate_order_total`, identify volume-based discounts with `get_tiered_unit_price`, verify wholesale eligibility via `validate_wholesale_order`, and generate comprehensive cost breakdowns using `bulk_order_summary`.


## Available Tools (4)
- **bulk_order_summary**: Provides a breakdown of costs for an order involving multiple different product types
- **calculate_order_total**: Calculates the total monetary value for a specific quantity and unit price
- **get_tiered_unit_price**: Determines the correct unit price based on a quantity and a set of pricing tiers
- **validate_wholesale_order**: Verifies if a specific order meets the minimum requirements for wholesale eligibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wholesale Order Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 50 units at $12.50 each?"

**🤖 AI Agent:**
> The total cost for 50 units at $12.50 each is $625.00.

---

**👤 You:**
> "Does an order of 15 units meet a minimum wholesale requirement of 20?"

**🤖 AI Agent:**
> No, the order is not eligible. You need 5 more units to meet the minimum requirement.

---

**👤 You:**
> "Give me a summary for an order with 10 units at $5 and 20 units at $3."

**🤖 AI Agent:**
> The order subtotal is $110.00, consisting of 2 unique items and a total quantity of 30 units.


## ❓ FAQ

**Q: How do I calculate the total for a bulk order?**
You can use the `calculate_order_total` tool by providing the quantity and the unit price.

**Q: Can I check if an order qualifies for wholesale pricing?**
Yes, use the `validate_wholesale_order` tool to check if the quantity meets the required threshold.

**Q: How does tiered pricing work?**
The `get_tiered_unit_price` tool evaluates the quantity against defined thresholds to return the most cost-effective unit price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wholesale-order-total](https://vinkius.com/en/ai-agent-connect/wholesale-order-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wholesale Order Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wholesale-order-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wholesale Order Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wholesale-order-total": {
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
