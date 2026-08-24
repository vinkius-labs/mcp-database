# Dew Point Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dew-point-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate dew point, wet-bulb temperature, and humidity metrics.

## Description
This MCP server provides a suite of psychrometric tools to analyze atmospheric conditions. Use `calculate_atmospheric_metrics` to determine dew point, wet-bulb temperature, absolute humidity, and vapor pressure. You can also use `get_comfort_status` to assess environmental comfort levels or `convert_humidity_units` to switch between measurement scales. It helps identify oppressive humidity or frost risks based on precise Magnus formula calculations.


## Available Tools (3)
- **calculate_atmospheric_metrics**: Provides a complete suite of psychrometric calculations based on current air conditions
- **convert_humidity_units**: Converts humidity metrics between different measurement scales
- **get_comfort_status**: Determines the qualitative comfort level of the environment based on dew point thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dew Point Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the atmospheric metrics for 25°C and 60% relative humidity."

**🤖 AI Agent:**
> The dew point is 16.66°C, the wet-bulb temperature is 18.12°C, absolute humidity is 12.45 g/m³, and vapor pressure is 19.23 hPa.

---

**👤 You:**
> "What is the comfort status for a dew point of 22°C?"

**🤖 AI Agent:**
> The comfort level is Oppressive and the risk category is High Humidity.

---

**👤 You:**
> "Convert 0.015 kg/m3 to g/m3."

**🤖 AI Agent:**
> 15 g/m3


## ❓ FAQ

**Q: How is the dew point calculated?**
The dew point is calculated using the Magnus formula with constants a=17.27 and b=237.7.

**Q: What are the risk thresholds?**
Conditions are flagged as 'Oppressive' if the dew point exceeds 20°C and as 'Frost Risk' if it falls below 0°C.

**Q: Which AI clients can use this tool?**
This tool is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dew-point-calculator](https://vinkius.com/ai-agent-connect/dew-point-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dew Point Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dew-point-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dew Point Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dew-point-calculator": {
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
