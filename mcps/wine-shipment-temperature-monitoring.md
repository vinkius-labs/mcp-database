# Wine Shipment Temperature Monitoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-shipment-temperature-monitoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate thermal risk, monitoring frequency, and data logger requirements for wine shipments.

## Description
This MCP server provides specialized intelligence for wine logistics. It allows AI agents to assess thermal stability risks using `get_excursion_risk` and adjust models via `evaluate_seasonal_routing_impact`. Agents can determine precise sensor needs using `calculate_monitoring_frequency` and `determine_logger_requirements` to ensure wine quality is maintained throughout transit.


## Available Tools (4)
- **determine_logger_requirements**: Specifies the hardware characteristics required to successfully monitor a specific shipment
- **evaluate_seasonal_routing_impact**: Adjusts the thermal exposure model based on the time of year the shipment is scheduled
- **get_excursion_risk**: Determines the probability and severity of temperature fluctuations during a specific transit route
- **calculate_monitoring_frequency**: Determines how often temperature readings must be taken to ensure data integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Shipment Temperature Monitoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the temperature excursion risk for a shipment of Fragile wine to Bordeaux for 10 days using standard packaging?"

**🤖 AI Agent:**
> The risk level for this shipment is Medium, with an estimated excursion duration of 4 hours due to the sensitivity of Fragile wine and standard packaging.

---

**👤 You:**
> "How often should I record temperatures for a High risk shipment lasting 72 hours?"

**🤖 AI Agent:**
> For a High risk shipment lasting 72 hours, the recording interval should be every 15 minutes, resulting in 288 total expected readings.

---

**👤 You:**
> "What logger do I need for a 5-day shipment with 15-minute intervals and 3 expected excursion events?"

**🤖 AI Agent:**
> You require a logger with at least 130 hours of battery life and a memory capacity of at least 480 readings. A high-precision digital sensor is recommended.


## ❓ FAQ

**Q: How does the tool account for different wine types?**
The `get_excursion_risk` tool uses the wine type to apply specific thermal sensitivity profiles, ensuring fragile wines receive stricter monitoring recommendations.

**Q: Can I plan for seasonal temperature changes?**
Yes, by using `evaluate_seasonal_routing_impact`, you can adjust the risk assessment based on the departure month and destination seasonality.

**Q: What hardware information is provided?**
The `determine_logger_requirements` tool provides specific hardware needs, including minimum battery life and memory capacity required for the shipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-shipment-temperature-monitoring](https://vinkius.com/en/ai-agent-connect/wine-shipment-temperature-monitoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Shipment Temperature Monitoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-shipment-temperature-monitoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Shipment Temperature Monitoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-shipment-temperature-monitoring": {
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
