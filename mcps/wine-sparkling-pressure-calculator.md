# Wine Sparkling Pressure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-sparkling-pressure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate CO2 pressure, required sugar, and nitrogen dilution for sparkling wine production.

## Description
This MCP server provides specialized calculation tools for sparkling wine producers using the Tirage or Charmat methods. It allows AI agents to determine internal CO2 pressure using `calculate_carbonation_pressure`, calculate the exact sugar needed for a target pressure with `calculate_required_sugar`, manage gas mixtures via `calculate_nitrogen_dilution`, and schedule production steps using `estimate_disgorgement_window`.


## Available Tools (4)
- **calculate_carbonation_pressure**: Determines the expected internal pressure based on current fermentation parameters
- **calculate_nitrogen_dilution**: Determines how much nitrogen gas is needed to dilute CO2 to a lower target pressure
- **calculate_required_sugar**: Calculates how much sugar must be added to achieve a specific target pressure
- **estimate_disgorgement_window**: Provides an estimate of when the wine will reach its target pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Sparkling Pressure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the pressure be if I have 10g/L sugar, 20°C, 500L liquid in a 600L tank?"

**🤖 AI Agent:**
> The calculated pressure is 2.45 bar with a CO2 concentration of 4.2 g/L.

---

**👤 You:**
> "How much sugar do I need to reach 5 bar in a 1000L tank at 15°C with 500L of liquid?"

**🤖 AI Agent:**
> You need to add 12.4 g/L of sugar to reach the target pressure of 5 bar.

---

**👤 You:**
> "How many days until I reach my target pressure if I have 15g/L sugar, a target of 5g/L, and a fermentation rate of 1.5g/L per day at 18°C?"

**🤖 AI Agent:**
> It will take approximately 6.67 days to reach the target pressure.


## ❓ FAQ

**Q: How do I calculate the pressure in my bottles?**
You can use the `calculate_carbonation_pressure` tool by providing the residual sugar, temperature, liquid volume, and total vessel volume.

**Q: Can I use this for the Charmat method?**
Yes, the server supports both Tirage and Charmat processes, including nitrogen dilution for tank fermentation.

**Q: How can I estimate when to disgorge?**
Use the `estimate_disgorgement_window` tool to predict the number of days remaining based on current sugar levels and fermentation rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-sparkling-pressure-calculator](https://vinkius.com/en/ai-agent-connect/wine-sparkling-pressure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Sparkling Pressure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-sparkling-pressure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Sparkling Pressure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-sparkling-pressure-calculator": {
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
