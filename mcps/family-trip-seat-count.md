# Family Trip Seat Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-trip-seat-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate vehicle capacity and passenger distribution for family trips.

## Description
This MCP server provides logistics tools to determine if a fleet of vehicles can safely accommodate a family. It handles complex seating requirements by accounting for adults, children, and infants, ensuring that child seat constraints and total vehicle capacities are respected. Use `calculate_total_fleet_capacity` to check overall availability, `find_optimal_vehicle_distribution` to plan passenger assignments, or `validate_safety_constraints` to verify specific vehicle setups.


## Available Tools (4)
- **calculate_total_fleet_capacity**: 
- **check_vehicle_capacity**: 
- **find_optimal_vehicle_distribution**: 
- **validate_safety_constraints**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Trip Seat Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can two SUVs with 7 seats each and 2 max child seats each carry 4 adults, 2 children, and 2 infants?"

**🤖 AI Agent:**
> Yes, the two SUVs provide a total of 14 seats and 4 child seat capacities, which is sufficient for 8 passengers including the 4 required child seats for the children and infants.

---

**👤 You:**
> "How should I distribute 2 adults, 3 children, and 1 infant across a Sedan (5 seats, 1 child seat) and a Minivan (7 seats, 3 child seats)?"

**🤖 AI Agent:**
> The optimal distribution is to place the infant and 1 child in the Minivan (using 2 child seats) and the remaining 2 children and 2 adults in the Sedan, or split them to ensure the child seat limit of the Sedan is not exceeded.

---

**👤 You:**
> "Is it safe to put 3 children and 1 infant in a car that only has 2 max child seats?"

**🤖 AI Agent:**
> No, that configuration is not safe because the total number of children and infants (4) exceeds the maximum child seat capacity of 2.


## ❓ FAQ

**Q: How does the tool handle infant seating?**
The tool treats infants as passengers requiring dedicated child seats. It uses `validate_safety_constraints` to ensure the number of infants and children does not exceed the vehicle's `maxChildSeats` limit.

**Q: Can I plan a trip for multiple vehicles?**
Yes, you can use `calculate_total_fleet_capacity` to aggregate the capacity of all your vehicles or `find_optimal_vehicle_distribution` to get a specific plan for your entire fleet.

**Q: What happens if a vehicle is unsafe for my group?**
The `check_vehicle_capacity` tool will return a seat warning or indicate that the configuration is not feasible if safety constraints like child seat limits are violated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-trip-seat-count](https://vinkius.com/en/ai-agent-connect/family-trip-seat-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Trip Seat Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-trip-seat-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Trip Seat Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-trip-seat-count": {
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
