# Moving Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate detailed moving costs for DIY, local, and full-service scenarios.

## Description
This MCP server provides precise financial planning for relocations. It calculates comprehensive cost breakdowns for three distinct service models: DIY, Local Mover, and Full-Service. Use `get_moving_estimate` to compare total costs and per-room expenses across these tiers. You can also use `validate_truck_capacity` to ensure your items fit the vehicle, `calculate_insurance_premium` to estimate protection costs, and `get_packing_needs` to determine the required quantity of boxes and tape.


## Available Tools (4)
- **calculate_insurance_premium**: Estimates the insurance cost based on the value of the items and the service level
- **get_moving_estimate**: Provides a comprehensive cost breakdown for the three primary service tiers
- **get_packing_needs**: Breaks down the required quantity and type of packing materials based on the volume of goods
- **validate_truck_capacity**: Determines if the provided volume and weight are compatible with standard moving vehicle types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the moving cost for a 500 cubic foot move with a distance of 100 miles, 20 hours of labor, and a $500 truck rate."

**🤖 AI Agent:**
> The estimated cost for your move is $1,250 for a Local Mover scenario, with a per-room cost of $250.

---

**👤 You:**
> "How many boxes and rolls of tape do I need for 300 cubic feet of items?"

**🤖 AI Agent:**
> You will need approximately 45 boxes and 5 rolls of tape for a volume of 300 cubic feet.

---

**👤 You:**
> "What is the insurance premium for a $10,000 shipment using Full-Service?"

**🤖 AI Agent:**
> The estimated insurance premium for a $10,000 value under the Full-Service tier is $150.


## ❓ FAQ

**Q: What service models are included in the estimates?**
The tool provides estimates for DIY (self-managed), Local Mover (hired labor/truck), and Full-Service (comprehensive professional moving) scenarios.

**Q: How does the tool handle unexpected expenses?**
The `get_moving_estimate` tool includes a contingency percentage that acts as a financial buffer for unforeseen circumstances like traffic or extra labor.

**Q: Can I check if my items will fit in a specific truck?**
Yes, you can use the `validate_truck_capacity` tool by providing the total volume and weight of your items to determine the appropriate truck type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-cost-estimator](https://vinkius.com/en/ai-agent-connect/moving-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-cost-estimator": {
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
