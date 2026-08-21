# Wind Chill Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wind-chill-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate perceived wind chill temperatures and frostbite risk levels.

## Description
This MCP server provides precise wind chill calculations based on the 2001 NWS/Environment Canada model. It allows AI agents to determine perceived temperatures and assess frostbite risks using the `calculate_wind_chill` tool. Users can also utilize `convert_units` to standardize measurements and `get_risk_thresholds` to understand safety classifications. It is designed to help users prepare for extreme cold conditions by providing estimated exposure times for skin damage.


## Available Tools (3)
- **calculate_wind_chill**: Calculates the perceived wind chill temperature and associated frostbite risks
- **convert_units**: Standardizes input values to the internal metric/imperial units
- **get_risk_thresholds**: Retrieves the constant definitions for frostbite risk categories and exposure times


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wind Chill Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the wind chill if it is 20°F with a wind speed of 15 mph?"

**🤖 AI Agent:**
> The wind chill is 3°F, which carries a Moderate frostbite risk.

---

**👤 You:**
> "Calculate wind chill for -10°C and 20 km/h wind."

**🤖 AI Agent:**
> The wind chill is 14°F, which carries a High frostbite risk.

---

**👤 You:**
> "Is there a risk at -60°F wind chill?"

**🤖 AI Agent:**
> Yes, a wind chill of -60°F is an extreme condition with an Extreme frostbite risk.


## ❓ FAQ

**Q: What formula is used for these calculations?**
The server uses the standardized 2001 model used by the National Weather Service (NWS) and Environment Canada.

**Q: When is wind chill applicable?**
Wind chill is calculated when the air temperature is at or below 50°F (10°C) and wind speed is greater than 3 mph.

**Q: Can I convert units using this server?**
Yes, you can use the `convert_units` tool to switch between Fahrenheit/Celsius and mph/kmh.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wind-chill-calculator](https://vinkius.com/ai-agent-connect/wind-chill-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wind Chill Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wind-chill-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wind Chill Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wind-chill-calculator": {
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
