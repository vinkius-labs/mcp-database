# Wine Distribution Margin Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-distribution-margin-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Models multi-tier wine pricing, cascading margins, and regulatory compliance.

## Description
This MCP server provides a specialized pricing engine for the wine industry. It models the standard three-tier distribution structure--Producer, Distributor, and Retailer--to calculate cascading margins and final retail costs. Users can use `calculate_full_chain_pricing` to get a complete breakdown from factory to shelf, including state-specific taxes. The engine also supports `get_state_regulatory_rules` to check for franchise state constraints and `apply_quantity_discount` to model volume-based savings. For sensitivity analysis, `simulate_margin_impact` allows users to see how changes in distributor or retailer markups affect the final consumer price.


## Available Tools (4)
- **simulate_margin_impact**: Simulates how changing a single margin tier affects the final consumer price
- **apply_quantity_discount**: Calculates how much the base price changes based on the volume ordered
- **calculate_full_chain_pricing**: Calculates the complete price breakdown from factory to shelf for a specific volume and location
- **get_state_regulatory_rules**: Retrieves specific legal constraints and tax rules for a given region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Distribution Margin Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the complete price breakdown for a wine with a $10 FOB price, 20% distributor margin, and 30% retailer margin in California?"

**🤖 AI Agent:**
> The distributor price is $12.00, the wholesale price is $15.60, and the final retail shelf price after California taxes is $18.45.

---

**👤 You:**
> "How much will I save if I order 500 units instead of 100 for a wine priced at $15.00 FOB?"

**🤖 AI Agent:**
> By increasing the order to 500 units, the discounted FOB price drops to $13.50, resulting in a total savings of $750.00.

---

**👤 You:**
> "If I increase the retailer margin from 30% to 35%, how much will the shelf price change for a $12.00 wholesale cost?"

**🤖 AI Agent:**
> Increasing the retailer margin by 5% will increase the final shelf price from $15.60 to $16.38, a difference of $0.78.


## ❓ FAQ

**Q: How does the three-tier model work?**
The model calculates costs by adding a margin at each stage: the Producer's FOB price is increased by the distributor's markup, and that total is then increased by the retailer's markup, while accounting for regional taxes.

**Q: Can I model direct shipping scenarios?**
Yes. By using `calculate_full_chain_pricing` with the direct shipping option enabled, the tool bypasses the distributor tier to model direct-to-consumer or direct-to-retailer flows.

**Q: Does this account for state-specific laws?**
Yes, the engine uses `get_state_regulatory_rules` to identify franchise state restrictions and apply the correct excise taxes and compliance fees for the target jurisdiction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-distribution-margin-calculator](https://vinkius.com/en/ai-agent-connect/wine-distribution-margin-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Distribution Margin Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-distribution-margin-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Distribution Margin Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-distribution-margin-calculator": {
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
