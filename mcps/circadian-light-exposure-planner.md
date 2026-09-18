# Circadian Light Exposure Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/circadian-light-exposure-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your circadian rhythm by planning strategic light exposure and restriction.

## Description
This MCP server helps you anchor your internal clock by managing light exposure. Use `plan_morning_exposure` to find the best time for morning light, `plan_evening_restriction` to identify when to dim lights for melatonin production, and `get_supplement_recommendations` to see if light therapy is needed. You can also use `evaluate_circadian_risk` to assess misalignment based on your environment and schedule.


## Available Tools (4)
- **evaluate_circadian_risk**: Assesses the risk of circadian misalignment based on the user's current environment and schedule
- **get_supplement_recommendations**: Recommends supplemental light devices when natural light is insufficient
- **plan_evening_restriction**: Identifies the window when light exposure should be minimized to ensure proper melatonin onset
- **plan_morning_exposure**: Determines the optimal timing and duration for morning light exposure to anchor the circadian rhythm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian Light Exposure Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I wake up at 07:00 and have access to both indoor and outdoor light. It is currently winter and my light level is 300 lux. When should I get light?"

**🤖 AI Agent:**
> You should begin your light exposure at 07:15. For the current winter conditions, a duration of 45 minutes is recommended to reach the target lux threshold.

---

**👤 You:**
> "I plan to go to bed at 22:30. My current evening light is 150 lux. When should I start dimming my lights?"

**🤖 AI Agent:**
> You should start reducing light intensity at 21:00. You should aim for a very dim environment to support melatonin onset.

---

**👤 You:**
> "I wake up at 06:00, go to bed at 23:00, and my average daily light is 200 lux in the summer. Is my rhythm okay?"

**🤖 AI Agent:**
> Your circadian risk score is 15, which indicates optimal alignment with your current environment and schedule.


## ❓ FAQ

**Q: How does this tool help my sleep?**
By using `plan_morning_exposure`, you can ensure you get enough light early in the day to suppress melatonin and trigger cortisol, which helps you stay alert and sleep better at night.

**Q: What if I live in a place with very little sunlight in winter?**
The `get_supplement_recommendations` tool specifically accounts for seasonal variations and can recommend light therapy devices to compensate for low winter light levels.

**Q: Can I check if my current schedule is healthy?**
Yes, you can use `evaluate_circadian_risk` to receive a risk score regarding your circadian misalignment based on your wake time, bedtime, and light intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/circadian-light-exposure-planner](https://vinkius.com/en/ai-agent-connect/circadian-light-exposure-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian Light Exposure Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circadian-light-exposure-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian Light Exposure Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-light-exposure-planner": {
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
