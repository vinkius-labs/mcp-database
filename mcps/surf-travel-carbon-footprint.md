# Surf Travel Carbon Footprint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-travel-carbon-footprint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Quantify and mitigate the carbon footprint of your surf trips.

## Description
This MCP server provides specialized carbon accounting tools for surfers to measure the environmental impact of their global travel. Use `calculate_trip_emissions` to find the CO2 produced by a single journey, `calculate_annual_impact` to project yearly footprints, `estimate_offset_cost` to determine neutralization costs, and `compare_sustainable_alternatives` to discover greener transport options.


## Available Tools (4)
- **calculate_annual_impact**: Scales a single trip's impact to a yearly footprint based on trip frequency
- **calculate_trip_emissions**: Determines the total CO2 emissions for a single journey based on mode and distance
- **compare_sustainable_alternatives**: Compares the current travel choice against greener options to suggest improvements
- **estimate_offset_cost**: Calculates the amount of carbon that needs to be offset and the estimated cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Travel Carbon Footprint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much CO2 is emitted for a 500km car trip?"

**🤖 AI Agent:**
> A 500km car trip emits 112.5 kg of CO2.

---

**👤 You:**
> "What is my annual footprint if I take four 1000km flights per year?"

**🤖 AI Agent:**
> Your total annual carbon footprint for these flights is 1,600 kg of CO2.

---

**👤 You:**
> "Is there a greener way to travel 200km than taking a car?"

**🤖 AI Agent:**
> Yes, switching to a train for a 200km trip would reduce your emissions significantly.


## ❓ FAQ

**Q: How do I calculate the impact of a single flight?**
You can use the `calculate_trip_emissions` tool by providing the transport mode as 'flight' and the total distance in kilometers.

**Q: Can I find cheaper ways to travel?**
Yes, use `compare_sustainable_alternatives` to see if switching from a flight to a train or car can reduce your CO2 emissions.

**Q: How much will it cost to offset my trip?**
Use `estimate_offset_cost` with the total emissions and the current market rate per kg of CO2 to get a precise USD estimate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-travel-carbon-footprint](https://vinkius.com/en/ai-agent-connect/surf-travel-carbon-footprint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Travel Carbon Footprint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-travel-carbon-footprint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Travel Carbon Footprint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-travel-carbon-footprint": {
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
