# Airport Transfer Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/airport-transfer-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise airport transfer costs based on distance and pricing tiers.

## Description
This MCP server provides a specialized calculation engine for airport transportation services. It allows AI agents to determine total trip costs by factoring in base fares and distance rates. Use `get_transfer_cost` to find specific trip prices, `validate_trip_feasibility` to check service area limits, `get_bulk_pricing_estimate` for multi-distance planning, and `compare_service_tiers` to evaluate different pricing models like Economy vs. Premium.


## Available Tools (4)
- **compare_service_tiers**: Compares two different pricing structures for the same distance
- **get_bulk_pricing_estimate**: Provides a range of costs for different distance tiers to help users plan
- **get_transfer_cost**: Calculates the final price for a specific trip
- **validate_trip_feasibility**: Checks if a requested distance is within the service area's capabilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airport Transfer Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost for a 25km trip with a $10 base fare and $2 per km rate?"

**🤖 AI Agent:**
> The total cost for the 25km trip is $60.

---

**👤 You:**
> "Is a 50km trip possible if the maximum service radius is 40km?"

**🤖 AI Agent:**
> No, the trip is not feasible as it exceeds the maximum service radius.

---

**👤 You:**
> "Compare an Economy tier ($5 base, $1.5/km) with a Premium tier ($20 base, $3/km) for a 10km trip."

**🤖 AI Agent:**
> The Economy tier costs $20 and the Premium tier costs $50. The Economy tier is cheaper.


## ❓ FAQ

**Q: How is the total transfer cost calculated?**
The total cost is the sum of the fixed base fare and the product of the total distance and the rate per kilometer.

**Q: Can I check if a driver can reach my location?**
Yes, you can use the `validate_trip_feasibility` tool to check if a requested distance is within the provider's maximum service radius.

**Q: How do I compare different vehicle tiers?**
You can use `compare_service_tiers` to compare the total cost of two different pricing structures for the same distance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/airport-transfer-cost-calculator](https://vinkius.com/en/ai-agent-connect/airport-transfer-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airport Transfer Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airport-transfer-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airport Transfer Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airport-transfer-cost-calculator": {
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
