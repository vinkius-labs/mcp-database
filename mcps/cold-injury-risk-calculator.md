# Cold Injury Risk Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cold-injury-risk-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess frostbite and hypothermia risks based on temperature, wind, and clothing.

## Description
This MCP server provides critical safety calculations for cold environments. It uses heat balance models and wind chill factors to determine physiological risks. Use `calculate_hypothermia_risk` to monitor core temperature drops, `calculate_frostbite_risk` to estimate time-to-injury for specific extremities like fingers or ears, and `get_exposure_limit_recommendation` for a conservative safety window. You can also use `compare_clothing_scenarios` to see how adding insulation affects your safety profile.


## Available Tools (4)
- **calculate_frostbite_risk**: Calculates the risk of frostbite for a specific body part
- **calculate_hypothermia_risk**: Calculates the risk of hypothermia based on environmental and physiological factors
- **compare_clothing_scenarios**: Compares the impact of adding clothing insulation on risk
- **get_exposure_limit_recommendation**: Provides a safe exposure limit recommendation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cold Injury Risk Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my hypothermia risk if it is -10°C with 5 m/s wind, wearing 1.5 clo, and I've been out for 30 minutes at a normal activity level?"

**🤖 AI Agent:**
> Your hypothermia risk score is 0.45, with an estimated core temperature of 36.2°C. Your recommended maximum exposure is 120 minutes.

---

**👤 You:**
> "How long until I get frostbite on my fingers at -15°C with 10 m/s wind and 0.5 clo insulation?"

**🤖 AI Agent:**
> Frostbite on your fingers is estimated to occur in 12 minutes, which is an Extreme risk level.

---

**👤 You:**
> "What happens to my safety limit if I add 1.0 clo of insulation at -5°C and 2 m/s wind?"

**🤖 AI Agent:**
> Adding 1.0 clo of insulation will reduce your risk by 35% and increase your safe exposure time from 45 minutes to 75 minutes.


## ❓ FAQ

**Q: How accurate are these risk assessments?**
The assessments use standard physiological heat balance models and wind chill formulas to provide estimates for safety planning.

**Q: Can I check risk for specific body parts?**
Yes, you can use `calculate_frostbite_risk` to check specific extremities like fingers, nose, or ears.

**Q: How does activity level affect the results?**
Higher activity levels increase metabolic heat production, which can mitigate some risks, but the tool accounts for this in all calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cold-injury-risk-calculator](https://vinkius.com/en/ai-agent-connect/cold-injury-risk-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cold Injury Risk Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cold-injury-risk-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cold Injury Risk Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cold-injury-risk-calculator": {
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
