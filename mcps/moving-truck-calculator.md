# Moving Truck Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/moving-truck-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate truck size, volume, weight, and moving supplies.

## Description
This MCP server provides deterministic logistics for moving operations. Use `calculate_move_requirements` to determine the recommended truck size, total volume, weight, and estimated fuel costs based on your home size and inventory. You can also use `estimate_packing_supplies` to find out how many tape rolls and bubble wrap units you need, or `validate_truck_capacity` to check if a specific vehicle can handle your load in one trip.


## Available Tools (3)
- **estimate_packing_supplies**: Calculates the quantity of consumable supplies needed based on the inventory
- **validate_truck_capacity**: Checks if a specific truck size is sufficient for the calculated volume
- **calculate_move_requirements**: Provides a comprehensive overview of the moving logistics including truck selection, volume, weight, and trips


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Truck Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am moving from a 1BR apartment with 5 large furniture items and 10 small boxes. The distance is 50 miles. What are my moving requirements?"

**🤖 AI Agent:**
> For a 1BR move with those items, you will need a 15ft truck. The total volume is estimated at 150 cubic feet, weighing approximately 1,050 lbs. You will need 1 trip, and the estimated fuel cost is $25.00.

---

**👤 You:**
> "How many tape rolls and bubble wrap units do I need for 20 boxes and 3 large furniture items?"

**🤖 AI Agent:**
> You will need 2 tape rolls and 3 units of bubble wrap.

---

**👤 You:**
> "Will a 10ft truck be enough for a 200 cubic foot load?"

**🤖 AI Agent:**
> No, a 10ft truck is not sufficient for a 200 cubic foot load; you will have a deficit of 190 cubic feet.


## ❓ FAQ

**Q: How do I know which truck size I need?**
You can use the `calculate_move_requirements` tool. It uses your home size and furniture count to recommend the best truck, such as a 15ft or 26ft vehicle.

**Q: Can I estimate my packing supply needs?**
Yes, the `estimate_packing_supplies` tool calculates the required tape rolls, bubble wrap, and packing paper based on your box and furniture counts.

**Q: How is fuel cost calculated?**
Fuel cost is calculated by multiplying the distance by the truck's MPG and the fuel price, then accounting for the number of trips required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/moving-truck-calculator](https://vinkius.com/ai-agent-connect/moving-truck-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Truck Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-truck-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Truck Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-truck-calculator": {
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
