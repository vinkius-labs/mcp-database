# Singapore ERP Toll Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-erp-toll-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact Singapore Electronic Road Pricing (ERP) costs for vehicles and routes.

## Description
This MCP server provides deterministic calculations for Singapore's Electronic Road Pricing (ERP) system. It allows AI agents to verify vehicle categories using `get_vehicle_validity`, determine specific toll costs for a single gantry via `get_single_gantry_toll`, or calculate the cumulative cost of a multi-gantry journey with `calculate_route_total_cost`. The tool uses fixed LTA rate cards to ensure precision for Cars, Motorcycles, Goods Vehicles, and Heavy Vehicles.


## Available Tools (3)
- **calculate_route_total_cost**: Calculate the cumulative cost of a journey passing through multiple gantries
- **get_single_gantry_toll**: Determine the cost of passing through one specific gantry at a specific time
- **get_vehicle_validity**: Verify if a provided vehicle category is recognized by the ERP system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore ERP Toll Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost for a Car to pass through gantry code 'A1' at 08:30?"

**🤖 AI Agent:**
> The toll cost for a Car at gantry A1 at 08:30 is 4.00 SGD.

---

**👤 You:**
> "Is 'Truck' a valid vehicle category for ERP?"

**🤖 AI Agent:**
> No, 'Truck' is not a recognized category. Please use 'Goods Vehicle' or 'Heavy Vehicle'.

---

**👤 You:**
> "What is the total cost for a Motorcycle passing through gantries B1, B2, and B3 at 14:00?"

**🤖 AI Agent:**
> The total cost for the route is 2.50 SGD.


## ❓ FAQ

**Q: How accurate are the toll calculations?**
The calculations are deterministic and based on fixed LTA rate cards, ensuring exact results for the specified vehicle category and time.

**Q: Which vehicle types are supported?**
The system supports Car, Motorcycle, Goods Vehicle, and Heavy Vehicle categories.

**Q: Can I calculate the cost for a whole trip?**
Yes, you can use the `calculate_route_total_cost` tool to find the total cost for a sequence of gantries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-erp-toll-calculator](https://vinkius.com/ai-agent-connect/singapore-erp-toll-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore ERP Toll Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-erp-toll-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore ERP Toll Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-erp-toll-calculator": {
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
