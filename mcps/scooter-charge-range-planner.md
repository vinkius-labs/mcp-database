# Scooter Charge & Range Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/scooter-charge-range-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Manage electric scooter energy constraints and trip feasibility.

## Description
This MCP server provides essential tools for managing electric scooter energy constraints. It allows AI agents to determine if planned trips are feasible based on current battery levels, safety reserves, and total range. Use `calculate_trip_feasibility` to check if a sequence of trips can be completed, `get_scooter_status_summary` for a high-level energy overview, `plan_optimized_charging` to simulate charging stops, and `validate_range_parameters` to ensure operational logic.


## Available Tools (4)
- **get_scooter_status_summary**: Provides a high-level overview of the current energy state and capacity
- **calculate_trip_feasibility**: Determines if a single trip or a sequence of trips can be completed given the current battery state
- **plan_optimized_charging**: Identifies if adding a charging stop at a specific point in a trip sequence would make an infeasible plan feasible
- **validate_range_parameters**: Validates a set of range-related constraints to ensure they are physically and operationally logical


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scooter Charge & Range Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can a scooter with 50% battery and a 60km full range complete two 12km trips with a 10% safety reserve?"

**🤖 AI Agent:**
> Yes, the trips are feasible. After accounting for the 10% safety reserve, the scooter has enough remaining charge to cover the 24km total distance.

---

**👤 You:**
> "Give me a summary of a scooter with 80% battery, 50km full range, and a 15% safety reserve."

**🤖 AI Agent:**
> The scooter has a usable range of 35km, a reserve range of 7.5km, and a total current range of 40km.

---

**👤 You:**
> "Is it possible to complete a 40km trip if the scooter has 30% battery and a 100km full range, with a 10% reserve?"

**🤖 AI Agent:**
> No, the trip is not feasible. The available range after the 10% reserve is only 20km, which is insufficient for a 40km trip.


## ❓ FAQ

**Q: How can I check if my scooter can complete a specific route?**
You can use the `calculate_trip_feasibility` tool by providing the current battery percentage, the total range of the scooter, and the distances of your planned trips.

**Q: What is the purpose of the safety reserve?**
The safety reserve is a mandatory battery percentage that must remain untouched to ensure the rider can safely reach a charging station or destination.

**Q: Can I simulate the effect of a charging stop?**
Yes, the `plan_optimized_charging` tool allows you to simulate adding a charge at a specific point in your trip sequence to see if it makes the plan feasible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/scooter-charge-range-planner](https://vinkius.com/en/ai-agent-connect/scooter-charge-range-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scooter Charge & Range Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scooter-charge-range-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scooter Charge & Range Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scooter-charge-range-planner": {
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
