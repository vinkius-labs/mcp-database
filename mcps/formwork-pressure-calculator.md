# Formwork Pressure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/formwork-pressure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates lateral pressure on formwork using ACI standards.

## Description
This MCP server provides engineering tools to calculate lateral pressure exerted by fresh concrete against formwork. It accounts for placement rates, concrete temperature, and vibration methods to ensure structural safety. Use `calculate_max_pressure` to find peak loads, `get_pressure_distribution` for vertical profiles, `calculate_tie_spacing` for reinforcement planning, and `analyze_mix_impact` to simulate how temperature or retarders change the pressure profile.


## Available Tools (4)
- **analyze_mix_impact**: Evaluates how changing specific variables (like temperature or retarders) affects the pressure
- **calculate_max_pressure**: Determines the peak lateral pressure exerted at the most critical point of the formwork
- **calculate_tie_spacing**: Determines the maximum allowable distance between formwork ties to prevent structural failure
- **get_pressure_distribution**: Provides a vertical profile of pressure at different depths to help engineers plan reinforcement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formwork Pressure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum pressure for a 5m pour at 2m/h with StandardMix and internal vibration?"

**🤖 AI Agent:**
> The maximum lateral pressure is 45.2 kPa, occurring at a critical height of 2.1 meters.

---

**👤 You:**
> "Show me the pressure distribution for a 3m pour with HighDensityMix."

**🤖 AI Agent:**
> The pressure profile shows a peak of 38.5 kPa at the base, decreasing to 12.2 kPa at the 3m mark.

---

**👤 You:**
> "How much will the pressure increase if I use retarders in my mix?"

**🤖 AI Agent:**
> Using retarders will increase the maximum pressure by 12.5% for this specific configuration.


## ❓ FAQ

**Q: How does the placement rate affect the results?**
A higher placement rate increases the time concrete behaves like a fluid, leading to higher peak pressure. You can use `calculate_max_pressure` to see how this affects your specific pour.

**Q: Can I calculate the required tie spacing?**
Yes, once you have the peak pressure, use `calculate_tie_spacing` to determine the maximum horizontal and vertical distances allowed between ties.

**Q: Does the tool account for chemical retarders?**
Yes, the `calculate_max_pressure` tool includes an optional parameter for retarders, which extends the fluid state of the concrete.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/formwork-pressure-calculator](https://vinkius.com/ai-agent-connect/formwork-pressure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formwork Pressure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formwork-pressure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formwork Pressure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formwork-pressure-calculator": {
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
