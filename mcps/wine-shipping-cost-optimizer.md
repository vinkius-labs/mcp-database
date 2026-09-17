# Wine Shipping Cost Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-shipping-cost-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Find the most cost-effective shipping methods for wine orders.

## Description
This MCP server provides tools to minimize logistics expenses for wine distributors. It calculates the ideal carrier, packaging, and route combinations by analyzing destination zones, package weights, and carrier rates. The system accounts for specialized requirements like temperature-controlled transit, insurance for declared value, and mandatory adult signatures. Use `optimize_shipping_plan` to find the single best configuration for an order, or `get_carrier_rates` to view available pricing for a specific region.


## Available Tools (4)
- **evaluate_shipping_option**: 
- **get_carrier_rates**: 
- **calculate_package_specs**: 
- **optimize_shipping_plan**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Shipping Cost Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cheapest way to ship 12 bottles of wine to zone North-East with a value of $300, requiring temperature control and an adult signature?"

**🤖 AI Agent:**
> The most cost-effective option is using Carrier Express with the Bulk Format package, totaling $45.50 per order.

---

**👤 You:**
> "Show me the available shipping rates for the West Coast zone."

**🤖 AI Agent:**
> The available rates for the West Coast zone are: Standard Ground at $12.00, Premium Express at $25.00, and Climate-Controlled at $38.00.

---

**👤 You:**
> "How much will a 6-pack of wine weigh in a Small Format box?"

**🤖 AI Agent:**
> A 6-pack in a Small Format box will have a total weight of 14.5 lbs.


## ❓ FAQ

**Q: How does the optimizer handle temperature-sensitive wine?**
The `evaluate_shipping_option` tool includes a premium for temperature-controlled transit to ensure wine remains at safe temperatures during shipping.

**Q: Can I compare different package types?**
Yes, you can use `calculate_package_specs` to find the weight and volume of different boxes, or use `optimize_shipping_plan` to automatically compare multiple package types.

**Q: Does this account for legal requirements like adult signatures?**
Yes, the system includes costs for mandatory adult signatures and insurance for the declared value of the shipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-shipping-cost-optimizer](https://vinkius.com/en/ai-agent-connect/wine-shipping-cost-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Shipping Cost Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-shipping-cost-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Shipping Cost Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-shipping-cost-optimizer": {
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
