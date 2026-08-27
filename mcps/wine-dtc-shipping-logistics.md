# Wine DTC Shipping & Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-dtc-shipping-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate DTC wine shipping costs, packaging expenses, and carrier comparisons.

## Description
This MCP server provides specialized tools for Direct-to-Consumer (DTC) wine logistics. It allows AI agents to calculate precise shipping costs using carrier rate cards, determine packaging material expenses based on bottle quantity, and compute total fulfillment costs including mandatory adult signature surcharges. Users can also use `compare_carrier_options` to identify the most cost-effective carrier for any given shipment profile, ensuring efficient logistics management for wine distributors.


## Available Tools (4)
- **calculate_packaging_cost**: Determines the cost of the materials required to ship the wine
- **calculate_shipping_cost**: Determines the base carrier cost for a specific shipment
- **calculate_total_fulfillment_cost**: Calculates the absolute total cost to fulfill an order, including all logistics and materials
- **compare_carrier_options**: Identifies the cheapest carrier for a specific shipment profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine DTC Shipping & Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total fulfillment cost for shipping 6 bottles to zone 4 using FedEx with a 6-pack box?"

**🤖 AI Agent:**
> The total fulfillment cost for 6 bottles to zone 4 using FedEx is $28.50, which includes a $15.00 base rate, $6.50 for the 6-pack packaging, and a $7.00 adult signature surcharge.

---

**👤 You:**
> "Which carrier is cheapest for 12 bottles to zone 2 using 12-pack packaging?"

**🤖 AI Agent:**
> UPS is the cheapest option for this shipment with a total cost of $42.00.

---

**👤 You:**
> "How much does the packaging cost for a single bottle?"

**🤖 AI Agent:**
> The material cost for single bottle packaging is $2.25.


## ❓ FAQ

**Q: How are shipping costs calculated?**
Costs are determined by the `calculate_shipping_cost` tool, which uses the destination zone, bottle quantity, and the specific carrier's rate card, including mandatory adult signature fees.

**Q: Can I compare different shipping carriers?**
Yes, the `compare_carrier_options` tool evaluates multiple carriers to find the lowest total fulfillment cost for your specific shipment profile.

**Q: Does this include packaging costs?**
Yes, you can use `calculate_packaging_cost` to find material expenses or `calculate_total_fulfillment_cost` to get a complete breakdown including shipping, packaging, and signature fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-dtc-shipping-logistics](https://vinkius.com/ai-agent-connect/wine-dtc-shipping-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine DTC Shipping & Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-dtc-shipping-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine DTC Shipping & Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-dtc-shipping-logistics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
