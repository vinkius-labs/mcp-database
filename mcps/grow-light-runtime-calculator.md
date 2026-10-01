# Grow Light Runtime Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grow-light-runtime-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Calculate supplemental lighting hours and electrical costs for indoor plants.

## Description
This MCP server provides precise tools for indoor growers to manage lighting schedules and energy expenses. Use `calculate_supplemental_runtime` to determine how much artificial light is needed to reach a target photoperiod based on available daylight. You can use `generate_lighting_schedule` to create a daily timing plan, `calculate_energy_consumption` to estimate electricity usage, and `calculate_operational_cost` to project monthly expenses.


## Available Tools (4)
- **calculate_energy_consumption**: Estimates the total electricity used by the lighting system
- **calculate_operational_cost**: Translates energy consumption into a predictable monetary expense
- **calculate_supplemental_runtime**: Determines how many hours of artificial light are needed to meet the plant's biological requirements
- **generate_lighting_schedule**: Provides a specific daily timing plan for when the grow lights should turn on and off


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grow Light Runtime Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 6 hours of natural sunlight and I need a 14-hour photoperiod. How many supplemental hours do I need?"

**🤖 AI Agent:**
> You need 8 hours of supplemental lighting.

---

**👤 You:**
> "What is the daily cost if I use 50 kWh per day and my electricity price is $0.15 per kWh?"

**🤖 AI Agent:**
> The daily cost is $7.50.

---

**👤 You:**
> "Calculate the energy use for 4 lights at 150W each running for 12 hours a day."

**🤖 AI Agent:**
> The daily energy consumption is 7.2 kWh.


## ❓ FAQ

**Q: How do I calculate the extra light needed?**
Use the `calculate_supplemental_runtime` tool by providing your available daylight hours and your target photoperiod.

**Q: Can I estimate my monthly electricity bill?**
Yes, use `calculate_energy_consumption` to find your daily usage, then use `calculate_operational_cost` with your local energy price to find the monthly total.

**Q: What information is needed for a lighting schedule?**
To use `generate_lighting_schedule`, you need the available daylight hours, the target photoperiod, and the time of sunrise.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grow-light-runtime-calculator](https://vinkius.com/en/ai-agent-connect/grow-light-runtime-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grow Light Runtime Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grow-light-runtime-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grow Light Runtime Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grow-light-runtime-calculator": {
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
