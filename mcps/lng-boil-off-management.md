# LNG Boil-Off Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lng-boil-off-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Predict and manage LNG boil-off rates, reliquefaction needs, and fuel consumption.

## Description
This MCP server provides specialized calculation tools for maritime LNG transport. It allows AI agents to determine the daily boil-off rate using `calculate_daily_bor`, estimate the necessary capacity for reliquefaction with `estimate_reliquefaction_needs`, and evaluate the balance between gas production and engine demand via `analyze_fuel_consumption_balance`. It also enables predicting total cargo loss over a voyage using `predict_voyage_cargo_loss`.


## Available Tools (4)
- **analyze_fuel_consumption_balance**: Evaluates the balance between BOG produced, BOG used for propulsion, and BOG that must be reliquefied
- **calculate_daily_bor**: Determines the daily amount of gas evaporated based on tank properties and environment
- **estimate_reliquefaction_needs**: Calculates the capacity required for a reliquefaction plant to handle the produced BOG
- **predict_voyage_cargo_loss**: Estimates the total volume of LNG lost or consumed over the entire journey


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LNG Boil-Off Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the daily boil-off for a 145,000 m3 tank with an insulation factor of 0.05 at 30°C ambient and -162°C cargo?"

**🤖 AI Agent:**
> The daily boil-off volume is 14.5 m3, with a daily mass of 7,250 kg and a rate of 0.01%.

---

**👤 You:**
> "Estimate the reliquefaction needs for a voyage of 20 days with a daily boil-off of 15 m3."

**🤖 AI Agent:**
> The required plant capacity is 15.5 m3 per day to handle the daily production with a safety margin.

---

**👤 You:**
> "Will I lose much cargo on a 15-day voyage with a 0.1% daily boil-off rate and 100,000 m3 initial volume?"

**🤖 AI Agent:**
> The total volume lost will be 1,500 m3, leaving a remaining cargo volume of 98,500 m3.


## ❓ FAQ

**Q: How do I calculate the daily evaporation rate?**
You can use the `calculate_daily_bor` tool by providing the tank volume, insulation factor, ambient temperature, and cargo temperature.

**Q: Can I check if my reliquefaction plant is sufficient?**
Yes, use `estimate_reliquefaction_needs` to determine the required plant capacity based on daily boil-off and voyage duration.

**Q: How is fuel consumption balanced against BOG?**
The `analyze_fuel_consumption_balance` tool evaluates the relationship between produced BOG, engine fuel demand, and reliquefaction capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lng-boil-off-management](https://vinkius.com/en/ai-agent-connect/lng-boil-off-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LNG Boil-Off Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lng-boil-off-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LNG Boil-Off Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lng-boil-off-management": {
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
