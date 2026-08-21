# Heat Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/heat-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate perceived temperature and heat-related health risks.

## Description
This MCP server provides precise calculations of the heat index (apparent temperature) using the NOAA Rothfusz regression. It helps determine how hot it actually feels by combining air temperature and relative humidity. The tool includes Steadman's adjustments for low humidity or specific high-temperature conditions to ensure accuracy. Use `get_heat_index` to find the perceived temperature and health risk level, or `get_risk_thresholds` to see the boundaries for caution levels.


## Available Tools (3)
- **get_heat_index**: Calculates the perceived temperature and determines the health risk level
- **get_risk_thresholds**: Retrieves the specific temperature and humidity boundaries used to define the different caution levels
- **validate_environmental_conditions**: Checks if a set of inputs falls into the specific atmospheric windows requiring Steadman's adjustment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heat Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the heat index if the temperature is 95°F and humidity is 60%?"

**🤖 AI Agent:**
> The heat index is 115°F, which falls under the Extreme Danger level.

---

**👤 You:**
> "Calculate the heat index for 30°C and 45% humidity."

**🤖 AI Agent:**
> The heat index is 86.3°F (30.2°C), which is categorized as Caution.

---

**👤 You:**
> "Is it dangerous to be outside at 85°F with 50% humidity?"

**🤖 AI Agent:**
> The heat index is 88°F, which is in the Caution level. It is generally manageable for most healthy individuals.


## ❓ FAQ

**Q: How accurate is the heat index calculation?**
The tool uses the NOAA Rothfusz regression and applies Steadman's adjustments for specific environmental conditions to provide highly accurate apparent temperature readings.

**Q: What are the caution levels?**
The caution levels include Caution, Extreme Caution, Danger, and Extreme Danger, based on the calculated heat index and associated physiological risks.

**Q: Can I use Celsius instead of Fahrenheit?**
Yes, you can specify the temperature unit as 'C' for Celsius or 'F' for Fahrenheit when using the tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/heat-index-calculator](https://vinkius.com/ai-agent-connect/heat-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heat Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heat-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heat Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heat-index-calculator": {
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
