# Transport Carbon Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transport-carbon-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate CO2 emissions for various transport modes including cars, planes, and trains.

## Description
Quantify the environmental impact of your travels. This MCP server provides tools like `estimate_trip_emissions`, `estimate_passenger_footprint`, and `compare_mode_efficiency` to calculate CO2 emissions based on distance, vehicle occupancy, and fuel types for modes such as car, plane, train, bus, motorcycle, and electric bike.


## Available Tools (3)
- **compare_mode_efficiency**: Compares multiple transport modes over the same distance to find the most efficient option
- **estimate_passenger_footprint**: Calculates the CO2 emission responsibility of a single individual in a shared trip
- **estimate_trip_emissions**: Calculates the total CO2 produced by a single vehicle for a specific distance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transport Carbon Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much CO2 is emitted for a 100km car trip using petrol?"

**🤖 AI Agent:**
> A 100km trip in a car using petrol produces 19000 grams of CO2.

---

**👤 You:**
> "What is the passenger footprint for a 500km flight with 2 people?"

**🤖 AI Agent:**
> The CO2 emission responsibility for each person is 150000 grams.

---

**👤 You:**
> "Compare car and train efficiency for a 200km trip."

**🤖 AI Agent:**
> The comparison shows that the train is more efficient, producing 1000 grams per person compared to 3800 grams for a car.


## ❓ FAQ

**Q: How does the calculator determine CO2 emissions?**
The calculation uses hardcoded emission factors per kilometer for each transport mode and fuel type, multiplied by the distance traveled.

**Q: Can I compare different modes of transport?**
Yes, you can use the `compare_mode_efficiency` tool to evaluate multiple modes over the same distance and find the most efficient option.

**Q: Does occupancy affect the results?**
Yes, using `estimate_passenger_footprint` allows you to see how sharing a vehicle with more passengers reduces the individual CO2 footprint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transport-carbon-calculator](https://vinkius.com/mcp/transport-carbon-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transport Carbon Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transport-carbon-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transport Carbon Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transport-carbon-calculator": {
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
