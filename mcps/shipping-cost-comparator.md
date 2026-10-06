# Shipping Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shipping-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Compare shipping rates, zones, and surcharges across multiple carriers.

## Description
This MCP server connects AI agents to logistics data, allowing for precise shipping cost analysis. Use `get_carrier_rates` to find the best quotes based on weight and dimensions, `calculate_zone_distance` to identify shipping zones, `get_surcharge_details` to see residential or fuel fees, and `compare_packaging_efficiency` to optimize package size for cost savings.


## Available Tools (4)
- **calculate_zone_distance**: Determine the shipping zone for a given origin and destination pair
- **compare_packaging_efficiency**: Evaluate how changing the package dimensions affects the final shipping cost across carriers
- **get_carrier_rates**: Retrieve a list of comparable shipping quotes from all available carriers for a specific package and route
- **get_surcharge_details**: Identify all potential surcharges applicable to a specific shipment profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipping Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare shipping rates for a 5kg package (30x30x30 cm) from 90210 to 10001 with a declared value of $100 using Express service."

**🤖 AI Agent:**
> Carrier A: $45.50, Carrier B: $42.00, Carrier C: $48.25. Carrier B is the cheapest option for Express service.

---

**👤 You:**
> "What is the shipping zone for a package sent from 90210 to 10001?"

**🤖 AI Agent:**
> The shipping zone for the route from 90210 to 10001 is Zone 8.

---

**👤 You:**
> "Will I save money if I reduce my package dimensions from 40x40x40 cm to 30x30x30 cm for a 2kg shipment?"

**🤖 AI Agent:**
> Yes, reducing the dimensions will save you $5.50 by decreasing the dimensional weight charge.


## ❓ FAQ

**Q: How do I compare rates between different carriers?**
You can use the `get_carrier_rates` tool by providing the package weight, dimensions, origin zip, destination zip, declared value, and desired service level.

**Q: Can I see if changing my package size will save money?**
Yes, the `compare_packaging_efficiency` tool evaluates how different dimensions impact the final cost and dimensional weight charges.

**Q: What kind of surcharges are included in the analysis?**
The `get_surcharge_details` tool provides a breakdown of residential fees, fuel surcharges, and oversized item fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shipping-cost-comparator](https://vinkius.com/en/ai-agent-connect/shipping-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipping Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shipping-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipping Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipping-cost-comparator": {
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
