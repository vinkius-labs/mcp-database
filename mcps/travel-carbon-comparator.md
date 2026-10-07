# Travel Carbon Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-carbon-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Quantify and compare the carbon footprint of different travel itineraries.

## Description
This MCP server provides tools to calculate and compare the environmental impact of travel. Use `compare_travel_scenarios` to evaluate multiple itineraries at once, or use `calculate_transport_emissions` and `calculate_lodging_emissions` for granular analysis of specific segments and stays. It accounts for distance, occupancy, cabin class, and lodging tiers to provide accurate CO2e metrics.


## Available Tools (4)
- **calculate_transport_emissions**: Determines the carbon impact for a single transportation segment
- **compare_travel_scenarios**: Compares the total carbon footprint between two or more defined travel itineraries
- **get_emission_factors**: Retrieves the current coefficient values for different modes and tiers
- **calculate_lodging_emissions**: Determines the carbon impact for a period of stay at a lodging facility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Carbon Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare two trips: Trip A is 500km by car with 2 people, and Trip B is 500km by train with 2 people."

**🤖 AI Agent:**
> Trip A (Car) has a total footprint of 85.5 kg CO2e, while Trip B (Train) has a total footprint of 12.2 kg CO2e. The train option reduces emissions by 73.3 kg CO2e.

---

**👤 You:**
> "What is the carbon impact of a 3-night stay in a luxury hotel for 1 person?"

**🤖 AI Agent:**
> The total carbon footprint for a 3-night stay in a luxury tier hotel is 45.0 kg CO2e.

---

**👤 You:**
> "Calculate emissions for a 1000km flight in Business class with 1 passenger."

**🤖 AI Agent:**
> The total carbon footprint for this flight segment is 350.0 kg CO2e.


## ❓ FAQ

**Q: How does cabin class affect the results?**
Cabin class changes the emission factor used in `calculate_transport_emissions`. Higher classes like Business or First Class have higher emission factors due to the space and weight allocated per passenger.

**Q: Can I compare multiple trips at once?**
Yes, you can use the `compare_travel_scenarios` tool to provide multiple itineraries and receive a comparison of their total CO2e footprints.

**Q: What factors are used for lodging emissions?**
Lodging emissions are calculated using the number of nights, the occupancy, and the lodging tier (e.g., Budget, Mid-range, Luxury) via the `calculate_lodging_emissions` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-carbon-comparator](https://vinkius.com/en/ai-agent-connect/travel-carbon-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Carbon Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-carbon-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Carbon Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-carbon-comparator": {
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
