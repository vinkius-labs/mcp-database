# Cold Stress Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cold-stress-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess hypothermia and frostbite risks based on environmental conditions.

## Description
This MCP server provides critical physiological safety assessments for cold environments. It calculates the wind chill equivalent temperature and uses it to estimate the time remaining before hypothermia or frostbite occurs. Users can evaluate risks by providing air temperature, wind speed, activity levels, and clothing insulation details. The server includes tools like `get_wind_chill`, `calculate_hypothermia_risk`, `assess_frostbite_danger`, and `get_clothing_recommendations` to provide actionable safety data.


## Available Tools (4)
- **assess_frostbite_danger**: Determines the risk and estimated time until frostbite occurs on exposed skin
- **calculate_hypothermia_risk**: Estimates the time remaining before a person reaches a dangerous state of core temperature drop
- **get_clothing_recommendations**: Suggests appropriate insulation levels to mitigate identified risks
- **get_wind_chill**: Determines the perceived temperature based on environmental conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cold Stress Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the wind chill if it is -10°C with a wind speed of 20 km/h?"

**🤖 AI Agent:**
> The wind chill equivalent temperature is -16.4°C.

---

**👤 You:**
> "How long until I face frostbite at -15°C wind chill if my clothes are wet?"

**🤖 AI Agent:**
> At a wind chill of -15°C with wet clothing, frostbite risk is high and could occur within 30 minutes.

---

**👤 You:**
> "I am sedentary in -5°C with 10 km/h wind. What clothing do I need?"

**🤖 AI Agent:**
> A recommended Clo value of 1.5 is suggested to maintain thermal comfort.


## ❓ FAQ

**Q: How accurate are the hypothermia risk estimates?**
The estimates are based on standard physiological models considering wind chill, metabolic heat, and insulation, but should be used as a guide alongside professional medical advice.

**Q: Does the tool account for wet clothing?**
Yes, the `calculate_hypothermia_risk` and `assess_frostbite_danger` tools specifically factor in wetness, which significantly accelerates heat loss.

**Q: Can I get clothing advice?**
Yes, you can use `get_clothing_recommendations` to receive specific insulation (Clo value) suggestions based on your current conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cold-stress-assessment](https://vinkius.com/en/ai-agent-connect/cold-stress-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cold Stress Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cold-stress-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cold Stress Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cold-stress-assessment": {
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
