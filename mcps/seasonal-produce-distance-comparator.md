# Seasonal Produce Distance Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seasonal-produce-distance-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Compare produce procurement options by calculating environmental and economic impact scores.

## Description
This MCP server provides decision-support tools to evaluate and rank produce procurement options. It calculates a weighted score based on transport emissions, storage energy requirements, and economic costs. Use `evaluate_produce_options` to rank multiple procurement scenarios at once, or use `calculate_transport_emissions` and `calculate_storage_energy_impact` for granular analysis of specific shipment legs.


## Available Tools (4)
- **calculate_transport_emissions**: Determines the carbon footprint specifically related to the movement of goods
- **evaluate_produce_options**: Calculates and ranks a list of produce procurement options based on user-defined priorities
- **get_transport_mode_factors**: Retrieves the constant emission intensity factors for different modes of transport
- **calculate_storage_energy_impact**: Calculates the environmental cost of maintaining the required temperature for the produce during transit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seasonal Produce Distance Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two apple shipments: Option A is 500kg via truck for 200km with chilled storage. Option B is 500kg via rail for 500km with ambient storage. Which is better for the environment?"

**🤖 AI Agent:**
> Option B is the better environmental choice due to the lower emission intensity of rail transport compared to truck, despite the longer distance.

---

**👤 You:**
> "Calculate the transport emissions for 1000kg of berries moved 1500km by air."

**🤖 AI Agent:**
> The transport emissions for 1000kg of berries over 1500km via air is 45000 carbon equivalent units.

---

**👤 You:**
> "What is the energy impact for 200kg of frozen produce stored for 48 hours?"

**🤖 AI Agent:**
> The energy impact for 200kg of frozen produce over 48 hours is 120 energy score units.


## ❓ FAQ

**Q: How does the tool calculate the environmental impact?**
The environmental impact is the sum of transport emissions, calculated via `calculate_transport_emissions`, and the energy required for storage, calculated via `calculate_storage_energy_impact`.

**Q: Can I prioritize cost over environmental impact?**
Yes. When using `evaluate_produce_options`, you can assign different weights to environmentalImpact, economicImpact, and logisticalSpeed to influence the final ranking.

**Q: What transport modes are supported?**
The tool supports various modes including sea, rail, truck, van, and air. You can retrieve the specific intensity factors using `get_transport_mode_factors`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seasonal-produce-distance-comparator](https://vinkius.com/en/ai-agent-connect/seasonal-produce-distance-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seasonal Produce Distance Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seasonal-produce-distance-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seasonal Produce Distance Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seasonal-produce-distance-comparator": {
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
