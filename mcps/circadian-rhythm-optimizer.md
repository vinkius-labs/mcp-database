# Circadian Rhythm Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/circadian-rhythm-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synchronize your daily schedule with your biological clock for peak performance.

## Description
This MCP server acts as a biological scheduling engine. It uses circadian biology to calculate optimal windows for meals, exercise, deep work, and sleep. By analyzing your chronotype and wake time, it provides precise guidance through tools like `get_optimal_daily_schedule` for a full daily blueprint, `get_light_exposure_plan` for light management, `get_metabolic_activity_sync` for nutritional timing, and `get_cognitive_performance_window` to identify peak alertness periods.


## Available Tools (4)
- **get_cognitive_performance_window**: Identifies the best times for high-stakes mental tasks
- **get_light_exposure_plan**: Provides specific instructions on when to seek bright light or darkness
- **get_metabolic_activity_sync**: Optimizes meal timing and exercise intensity based on metabolic rhythm
- **get_optimal_daily_schedule**: Generates a comprehensive daily blueprint of optimal activity windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian Rhythm Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I wake up at 07:00 and I am a morning lark. Can you give me a full daily schedule for muscle gain?"

**🤖 AI Agent:**
> Based on your 07:00 wake time and morning lark chronotype, your optimal schedule for muscle gain includes breakfast at 07:30, a high-intensity exercise window between 09:00 and 10:30, and a caffeine cutoff at 12:00.

---

**👤 You:**
> "I'm a night owl waking up at 09:00. When should I seek bright light?"

**🤖 AI Agent:**
> For a night owl waking at 09:00, you should seek bright light exposure between 09:15 and 10:00 to help advance your circadian phase.

---

**👤 You:**
> "When is my best time for deep work if I wake up at 08:00 and am an intermediate type?"

**🤖 AI Agent:**
> Your peak alertness window for deep work is between 10:00 and 12:30.


## ❓ FAQ

**Q: How does this tool help my productivity?**
It identifies your peak alertness windows using `get_cognitive_performance_window`, allowing you to schedule high-stakes mental tasks when your brain is most ready.

**Q: Can I optimize my workouts?**
Yes, you can use `get_metabolic_activity_sync` to align your exercise intensity and meal timing with your metabolic rhythm.

**Q: What is a chronotype?**
A chronotype is your internal biological clock pattern, such as being a Morning Lark or a Night Owl, which dictates your natural energy cycles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/circadian-rhythm-optimizer](https://vinkius.com/en/ai-agent-connect/circadian-rhythm-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian Rhythm Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circadian-rhythm-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian Rhythm Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-rhythm-optimizer": {
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
