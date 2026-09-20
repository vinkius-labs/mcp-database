# Wind-Down Duration Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wind-down-duration-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Personalized wind-down plans and relaxation strategies based on arousal levels.

## Description
This MCP server helps you prepare for sleep by calculating optimal wind-down periods. By analyzing your evening activity intensity, stress levels, and sleep history, it provides a complete plan using `calculate_wind_down_plan`. You can also use `get_relaxation_activity_suggestions` for specific tasks, `estimate_sleep_readiness` to check your current state, or `get_screen_free_guidelines` to know exactly when to put your devices away.


## Available Tools (4)
- **calculate_wind_down_plan**: Provides a comprehensive recommendation including duration, activities, and screen-free timing
- **estimate_sleep_readiness**: Estimates how prepared the user is for sleep based on activity and stress
- **get_relaxation_activity_suggestions**: Answers what specific things can be done to relax based on current arousal
- **get_screen_free_guidelines**: Provides guidelines and timing for a screen-free period before sleep


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wind-Down Duration Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I had a very intense workout and I'm feeling quite stressed. What should my wind-down plan look like?"

**🤖 AI Agent:**
> Based on your high activity and stress, you should follow a 60-minute wind-down period. Start your screen-free period at 21:00. Suggested activities include deep breathing and light stretching.

---

**👤 You:**
> "How ready am I for sleep if I've had low activity and low stress?"

**🤖 AI Agent:**
> Your sleep readiness score is 95. You are very well prepared for sleep.

---

**👤 You:**
> "When should I stop using my phone if I want to sleep at 23:00 and I had moderate activity?"

**🤖 AI Agent:**
> You should stop using screens at 22:00 to allow for a sufficient wind-down period.


## ❓ FAQ

**Q: How does the wind-down plan work?**
The system uses an arousal reduction model. It looks at your activity and stress to determine how much time you need to return to a state suitable for sleep.

**Q: Can I get specific relaxation ideas?**
Yes, you can use the `get_relaxation_activity_suggestions` tool to receive tailored activities based on your current arousal state.

**Q: What is a screen-free period?**
It is a dedicated window of time before sleep where you avoid digital devices to reduce cognitive stimulation and blue light exposure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wind-down-duration-recommender](https://vinkius.com/en/ai-agent-connect/wind-down-duration-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wind-Down Duration Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wind-down-duration-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wind-Down Duration Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wind-down-duration-recommender": {
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
