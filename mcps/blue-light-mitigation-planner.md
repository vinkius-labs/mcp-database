# Blue Light Mitigation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blue-light-mitigation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Creates personalized schedules to reduce blue light exposure and optimize sleep hygiene.

## Description
This MCP server provides a suite of tools to help users manage blue light exposure before sleep. Use `generate_mitigation_plan` to receive a complete schedule including when to wear glasses and adjust device settings. You can use `assess_device_risk` to evaluate the threat level of your hardware, `calculate_buffer_period` to find your ideal no-screen window, and `get_environment_optimization` to improve your physical lighting setup.


## Available Tools (4)
- **assess_device_risk**: Evaluates the cumulative blue light risk score for a specific hardware setup
- **calculate_buffer_period**: Determines the optimal duration of the pre-sleep "no-screen" window
- **generate_mitigation_plan**: Provides a comprehensive schedule of when to wear glasses, adjust device settings, and modify the environment
- **get_environment_optimization**: Suggests specific changes to the physical surroundings to minimize light pollution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blue Light Mitigation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to sleep at 23:00. I'll be gaming on my laptop and scrolling on my phone. What should my plan be?"

**🤖 AI Agent:**
> To prepare for your 23:00 bedtime, you should start wearing blue light blocking glasses at 20:00. Activate Night Shift on your laptop at 21:00. You must stop all screen usage by 22:15 to respect your buffer zone.

---

**👤 You:**
> "How much blue light risk am I facing if I use a desktop monitor and a smartphone in the evening?"

**🤖 AI Agent:**
> Your risk score is high due to the combination of a desktop monitor and smartphone usage.

---

**👤 You:**
> "Suggest some lighting changes for my bedroom which currently uses LED lights."

**🤖 AI Agent:**
> Dim the overhead lights and consider using amber-tinted bulbs to reach an optimal color temperature.


## ❓ FAQ

**Q: How do I get a full schedule?**
Use the `generate_mitigation_plan` tool with your target bedtime and planned activities to get a complete timeline.

**Q: Can I check the risk of my specific devices?**
Yes, use `assess_device_risk` by providing a list of your device types to see your cumulative blue light risk score.

**Q: What is a buffer period?**
It is the window of time before sleep where you should stop all screen usage. You can calculate this using `calculate_buffer_period`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blue-light-mitigation-planner](https://vinkius.com/en/ai-agent-connect/blue-light-mitigation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blue Light Mitigation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blue-light-mitigation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blue Light Mitigation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blue-light-mitigation-planner": {
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
