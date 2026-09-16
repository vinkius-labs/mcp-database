# Refinery Emission Inventory Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-emission-inventory-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify pollutant emissions from refinery operations using standardized emission factors.

## Description
This MCP server provides a specialized calculation engine for quantifying pollutant emissions within refinery environments. It integrates operational activity data with standardized emission factors, such as EPA AP-42, to provide precise inventory reports. Users can use `get_pollutant_summary` to view total emissions by species, `get_source_contribution` to identify primary emission sources, `calculate_fugitive_emissions` for equipment leak estimation, `calculate_tank_storage_losses` for storage tank analysis, and `get_emission_trends` to monitor historical pollutant changes over time.


## Available Tools (5)
- **calculate_fugitive_emissions**: Estimates emissions originating from equipment leaks rather than point sources
- **calculate_tank_storage_losses**: Quantifies emissions from storage tank operations, accounting for working and standing losses
- **get_emission_trends**: Analyzes how emission levels change over multiple time intervals
- **get_pollutant_summary**: Provides a high-level view of total emissions grouped by pollutant type
- **get_source_contribution**: ) are emitting a specific pollutant.

Identifies which specific emission sources are the primary contributors to the total inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Emission Inventory Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total emission summary for the current period?"

**🤖 AI Agent:**
> The total aggregate mass for the current period is 450.5 kg, with SO2 being the primary pollutant at 120.2 kg.

---

**👤 You:**
> "Which sources are contributing most to NOx emissions?"

**🤖 AI Agent:**
> The primary contributors to NOx are Stack_01 (45 kg) and Flare_Unit_B (30 kg).

---

**👤 You:**
> "Show me the monthly emission trends for VOCs."

**🤖 AI Agent:**
> VOC emissions for the last three months were: January (12 kg), February (15 kg), and March (14 kg).


## ❓ FAQ

**Q: How are emission factors determined?**
The engine uses a combination of Tier 1 regulatory factors from EPA AP-42 standards and Tier 2 operational factors derived from specific refinery hardware specifications.

**Q: Can I track specific equipment leaks?**
Yes, you can use `calculate_fugitive_emissions` to estimate mass released from equipment like valves or pumps based on leak counts.

**Q: Does this account for storage tank evaporation?**
Yes, the `calculate_tank_storage_losses` tool quantifies both working and standing losses for specific storage tanks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-emission-inventory-engine](https://vinkius.com/en/ai-agent-connect/refinery-emission-inventory-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Emission Inventory Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-emission-inventory-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Emission Inventory Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-emission-inventory-engine": {
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
