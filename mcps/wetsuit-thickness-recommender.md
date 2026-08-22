# Wetsuit Thickness Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wetsuit-thickness-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Get precise wetsuit thickness and gear recommendations based on water temperature, air temperature, wind chill, and session duration.

## Description
This MCP server provides deterministic thermal protection profiles for surfers, swimmers, and divers. By analyzing the interaction between water temperature and wind-chill adjusted air temperature, it calculates an effective temperature to determine the most critical thermal threat. Use `calculate_wetsuit_recommendation` to receive a full profile including suit thickness (e.g., 3/2mm, 4/3mm) and necessary accessories like hoods or gloves. The tool also accounts for session endurance, automatically suggesting thicker insulation for sessions exceeding 2 hours.


## Available Tools (3)
- **get_thermal_risk_summary**: Analyzes the environmental conditions to provide a simplified risk assessment
- **calculate_wetsuit_recommendation**: Provides a complete thermal protection profile including suit thickness and necessary accessories
- **validate_session_parameters**: Checks if the provided environmental and duration data are within logical bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wetsuit Thickness Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm going surfing in 18°C water, 15°C air, with 20km/h wind for a 3-hour session. What wetsuit do I need?"

**🤖 AI Agent:**
> You should use a 4/3mm wetsuit. Because your session is longer than 2 hours, an endurance adjustment was applied to the base 3/2mm recommendation.

---

**👤 You:**
> "What is the thermal risk if the water is 12°C and the air is 10°C with 5km/h wind?"

**🤖 AI Agent:**
> The effective temperature is 10°C. This is considered cold water, and you will likely need a 5/4/3mm wetsuit along with a hood, booties, and gloves.

---

**👤 You:**
> "Recommend gear for 25°C water and 25°C air with no wind for a 1-hour swim."

**🤖 AI Agent:**
> A 0-2mm spring suit is recommended for these warm conditions.


## ❓ FAQ

**Q: How does wind speed affect my wetsuit recommendation?**
Wind speed increases heat loss through wind chill. The tool adjusts the air temperature downward based on wind speed to find the effective temperature, which may lead to a recommendation for a thicker suit.

**Q: Does the tool consider how long I will be in the water?**
Yes. If your planned session duration exceeds 2 hours, the `calculate_wetsuit_recommendation` tool applies an endurance adjustment, recommending a suit that is 1mm thicker to prevent heat loss during prolonged exposure.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP server to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wetsuit-thickness-recommender](https://vinkius.com/ai-agent-connect/wetsuit-thickness-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wetsuit Thickness Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wetsuit-thickness-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wetsuit Thickness Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wetsuit-thickness-recommender": {
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
