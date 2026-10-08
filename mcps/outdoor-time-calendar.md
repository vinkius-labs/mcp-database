# Outdoor Time Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outdoor-time-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules outdoor activities based on daylight, weather, and availability.

## Description
This MCP server helps you plan outdoor activities by analyzing daylight windows, weather suitability, and your personal availability. Use `get_available_slots` to find perfect times for your activities, `calculate_weekly_progress` to track your outdoor goals, and `suggest_optimal_schedule` to receive tailored recommendations for hitting your weekly targets. It ensures your activities align with both the sun and the weather.


## Available Tools (4)
- **calculate_weekly_progress**: Determines how much of the user's weekly goal has been met and how much remains
- **get_available_slots**: Identifies all possible time windows where a user can perform a specific activity
- **suggest_optimal_schedule**: Recommends the best upcoming times to perform activities to hit the weekly target
- **validate_weather_suitability**: Checks if a specific weather condition allows for outdoor activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outdoor Time Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me available slots for a 60-minute run tomorrow between 8 AM and 12 PM, given the sun is up from 6 AM to 8 PM and the weather is sunny."

**🤖 AI Agent:**
> I found two valid 60-minute slots for your run: 08:00 to 09:00 and 10:00 to 11:00.

---

**👤 You:**
> "I want to spend 5 hours outdoors this week. I have already completed two 45-minute sessions. How much progress have I made?"

**🤖 AI Agent:**
> You have completed 1.5 hours so far, which is 30% of your 5-hour weekly goal. You have 3.5 hours remaining.

---

**👤 You:**
> "Is it a good time for photography if the weather is stormy?"

**🤖 AI Agent:**
> No, stormy weather is typically not suitable for photography activities.


## ❓ FAQ

**Q: How does the tool determine if a time slot is valid?**
A slot is valid if it is fully contained within both a daylight window and your provided availability windows, and the weather is deemed suitable for your activity.

**Q: Can I prioritize certain times of day?**
Yes, you can use `suggest_optimal_schedule` with a priority window like 'morning' or 'afternoon' to get better recommendations.

**Q: How do I track my weekly outdoor goals?**
You can use `calculate_weekly_progress` by providing your target hours and a list of completed activity durations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outdoor-time-calendar](https://vinkius.com/en/ai-agent-connect/outdoor-time-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outdoor Time Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outdoor-time-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outdoor Time Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outdoor-time-calendar": {
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
