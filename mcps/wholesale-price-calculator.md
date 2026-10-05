# Wholesale Price Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wholesale-price-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A precision pricing engine for calculating optimal wholesale prices.

## Description
This MCP server provides a precision pricing engine designed to balance manufacturing costs, target manufacturer margins, shipping overhead, and retailer requirements. It allows AI agents to determine the ideal wholesale price per unit by analyzing COGS, shipping impact, and margin constraints. Use `calculate_wholesale_price` to find the optimal price point, `validate_margin_feasibility` to check if a price meets all stakeholder needs, `calculate_shipping_impact` to see how order volume affects unit costs, and `get_pricing_tier_summary` to retrieve default settings for Economy, Standard, or Premium tiers.


## Available Tools (4)
- **calculate_wholesale_price**: Determines the optimal wholesale price per unit that satisfies both manufacturer profit targets and retailer margin constraints
- **calculate_shipping_impact**: Determines how the shipping cost affects the unit economics based on order volume
- **get_pricing_tier_summary**: g., Economy, Standard, Premium).

Retrieves the configuration settings for different product tiers
- **validate_margin_feasibility**: Checks if a specific wholesale price is compatible with the manufacturer's profit goals and the retailer's margin needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wholesale Price Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the wholesale price for a product with a $50 unit cost, 20% manufacturer margin, 40% retailer margin, $500 total shipping, 100 unit MOQ, and a $100 target retail price."

**🤖 AI Agent:**
> The optimal wholesale price is $62.50, which is viable for both the manufacturer and the retailer.

---

**👤 You:**
> "How much does shipping add to each unit if the total cost is $200 and the order quantity is 50 units?"

**🤖 AI Agent:**
> The per-unit shipping cost is $4.00.

---

**👤 You:**
> "What are the default settings for the Premium tier?"

**🤖 AI Agent:**
> The Premium tier features a high standard margin, a high minimum order quantity, and significant shipping multipliers.


## ❓ FAQ

**Q: How does the tool handle shipping costs?**
The tool calculates per-unit shipping impact by dividing the total shipping cost by the minimum order quantity, ensuring accurate unit economics.

**Q: Can I check if a specific price is profitable for both parties?**
Yes, you can use `validate_margin_feasibility` to verify if a proposed wholesale price satisfies both the manufacturer's profit goals and the retailer's margin requirements.

**Q: What are the available pricing tiers?**
The system includes Economy, Standard, and Premium tiers, which can be queried using `get_pricing_tier_summary` to retrieve default margins and MOQs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wholesale-price-calculator](https://vinkius.com/en/ai-agent-connect/wholesale-price-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wholesale Price Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wholesale-price-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wholesale Price Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wholesale-price-calculator": {
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
