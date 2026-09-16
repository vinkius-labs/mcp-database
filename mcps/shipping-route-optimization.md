# Shipping Route Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shipping-route-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize maritime routes for tankers using weather-aware routing and fuel efficiency calculations.

## Description
This MCP server provides specialized maritime logistics tools for oil and gas tankers. It connects AI agents to real-time environmental data and vessel-specific constraints. Use `get_optimal_route` to find the most efficient path between ports, `analyze_weather_impact` to assess safety risks from waves and wind, `calculate_vessel_consumption` to predict fuel burn, and `check_route_compliance` to ensure routes respect maritime restrictions and draft limits.


## Available Tools (4)
- **get_optimal_route**: Calculates the most efficient path between two points considering all environmental and vessel constraints
- **analyze_weather_impact**: Evaluates how current or forecasted weather conditions along a specific route will affect vessel performance
- **calculate_vessel_consumption**: Predicts fuel usage based on vessel-specific efficiency curves and environmental resistance
- **check_route_compliance**: Validates that a proposed route does not violate maritime restrictions or vessel draft constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipping Route Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the most fuel-efficient route from Port of Rotterdam to Port of Singapore for vessel TANKER-99."

**🤖 AI Agent:**
> The optimal fuel-efficient route for TANKER-99 from Rotterdam to Singapore covers 8,450 nautical miles with an estimated arrival on October 12th, 2024, consuming 1,240 metric tons of fuel.

---

**👤 You:**
> "Is the route [0,0, 10,10, 20,20] safe for vessel TANKER-42 given current weather?"

**🤖 AI Agent:**
> The route has a safety score of 85. The primary weather risk identified is Strong Headwinds, which may cause an expected delay of 4 hours.

---

**👤 You:**
> "Check if the route through the Suez Canal is compliant for vessel TANKER-77."

**🤖 AI Agent:**
> The route is compliant. No violations of restricted areas or draft constraints were detected for TANKER-77.


## ❓ FAQ

**Q: How does the routing prioritize fuel efficiency?**
When the `get_optimal_route` tool is called with the priority set to 'fuel', it selects paths that utilize favorable ocean currents and minimize wave resistance to reduce total consumption.

**Q: Can I check if a route is safe for a specific tanker?**
Yes, you can use `analyze_weather_impact` to get a safety score based on weather conditions, or `check_route_compliance` to verify that the route respects vessel draft and restricted zones.

**Q: What factors affect the fuel consumption calculation?**
The `calculate_vessel_consumption` tool calculates fuel burn based on the specific vessel's efficiency profile, the intended speed over ground, and environmental resistance from waves and currents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shipping-route-optimization](https://vinkius.com/en/ai-agent-connect/shipping-route-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipping Route Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shipping-route-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipping Route Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipping-route-optimization": {
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
