# Shipping Zone Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/shipping-zone-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise freight costs using dimensional weight and shipping zones.

## Description
This MCP server provides deterministic freight cost estimation by calculating dimensional weight, identifying shipping zones, and applying carrier rate matrices. Use `get_dimensional_weight` to find volumetric weight, `determine_shipping_zone` to map zip codes to zones, and `calculate_freight_cost` to determine the final billable weight and total cost.


## Available Tools (3)
- **calculate_freight_cost**: Determines the final shipping cost using the billable weight, target zone, and carrier rates
- **determine_shipping_zone**: Identifies the target shipping zone based on the relationship between origin and destination locations
- **get_dimensional_weight**: Calculates the volumetric weight of a package based on its physical dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipping Zone Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the dimensional weight for a package that is 50x40x30 cm with a dim factor of 5000?"

**🤖 AI Agent:**
> The dimensional weight is 12 kg.

---

**👤 You:**
> "Calculate the shipping cost for a 10kg package with a 12kg dimensional weight in zone 3 using this rate matrix: {"3": [{"maxWeight": 15, "cost": 25.00}]}"

**🤖 AI Agent:**
> The billable weight is 12 kg, the zone is 3, and the total cost is $25.00.

---

**👤 You:**
> "Find the shipping zone for origin 90210 and destination 10001 using the map: {"90210-10001": 5}"

**🤖 AI Agent:**
> The target shipping zone is 5.


## ❓ FAQ

**Q: How is the billable weight determined?**
The billable weight is the higher value between the actual physical weight and the dimensional weight calculated via `get_dimensional_weight`.

**Q: Can I use my own carrier rates?**
Yes, you can provide your own rate matrix to the `calculate_freight_cost` tool to get exact pricing based on your specific carrier contracts.

**Q: What information is needed to find a shipping zone?**
You need the origin zip code, the destination zip code, and a zone map provided to the `determine_shipping_zone` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/shipping-zone-cost-calculator](https://vinkius.com/ai-agent-connect/shipping-zone-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipping Zone Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shipping-zone-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipping Zone Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipping-zone-cost-calculator": {
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
