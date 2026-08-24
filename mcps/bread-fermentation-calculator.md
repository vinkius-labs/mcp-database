# Bread Fermentation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bread-fermentation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic scheduling for bread fermentation timing and temperature.

## Description
This MCP server provides precise fermentation scheduling by calculating bulk fermentation duration, proofing time, and target dough temperatures. It accounts for yeast activity tiers, thermal management via friction factors, and cold retard adjustments to ensure consistent bread production.


## Available Tools (3)
- **calculate_cold_retard_adjustment**: Calculates how much fermentation is slowed when moving dough to a cold environment
- **calculate_fermentation_schedule**: Provides the complete timeline for bread production based on thermal and yeast inputs
- **calculate_water_temperature**: Determines the necessary water temperature to hit a target dough temperature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bread Fermentation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to hit a target dough temperature of 26°C. The room is 22°C and I expect 7°C of heat from mixing. What water temperature do I need?"

**🤖 AI Agent:**
> You need to use water at 23°C.

---

**👤 You:**
> "Calculate a schedule for 25°C dough using instant yeast (2% quantity) for a 4 hour fermentation."

**🤖 AI Agent:**
> Your bulk fermentation will take 4.0 hours, proofing will take 1.5 hours, and your target dough temperature is 25°C.

---

**👤 You:**
> "My dough is at 24°C and I'm putting it in a 4°C fridge. It is 50% through bulk fermentation. How much extra time is needed?"

**🤖 AI Agent:**
> You will need an additional 12.5 hours at the cold temperature to complete fermentation.


## ❓ FAQ

**Q: How does temperature affect my fermentation schedule?**
The `calculate_fermentation_schedule` tool applies a kinetic correction factor where yeast activity roughly doubles for every 8°C increase in dough temperature.

**Q: How do I calculate the correct water temperature?**
You can use `calculate_water_temperature` to determine the required water temperature by providing your target dough temperature, room temperature, and the friction factor from mixing.

**Q: Can I plan for overnight cold fermentation?**
Yes, the `calculate_cold_retard_adjustment` tool calculates the additional time needed when moving dough to a cold environment like a refrigerator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bread-fermentation-calculator](https://vinkius.com/ai-agent-connect/bread-fermentation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bread Fermentation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bread-fermentation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bread Fermentation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bread-fermentation-calculator": {
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
