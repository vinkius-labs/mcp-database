# Meditation Retreat Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meditation-retreat-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured meditation retreat schedules and silence policies.

## Description
This MCP server provides specialized tools for planning meditation retreats. It helps practitioners and organizers design balanced schedules by calculating sitting periods, walking meditation, and meal timings based on tradition type and intensity. Use `get_retreat_schedule` to create a full hourly itinerary, `get_silence_policy` to determine Noble Silence requirements, `calculate_daily_rhythm` to see time allocations, and `validate_retreat_feasibility` to ensure the plan is appropriate for the practitioner's experience level.


## Available Tools (4)
- **calculate_daily_rhythm**: Provides a summarized view of the daily patterns
- **get_retreat_schedule**: Generates a complete, hourly schedule for a specified retreat duration
- **get_silence_policy**: Determines the nature and duration of Noble Silence periods
- **validate_retreat_feasibility**: Checks if a requested retreat configuration is sustainable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meditation Retreat Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you create a 3-day intensive Vipassana retreat schedule for an intermediate practitioner?"

**🤖 AI Agent:**
> Here is your 3-day intensive Vipassana schedule: Day 1 starts with 2 hours of sitting, followed by 30 minutes of walking meditation, and continues with structured meal times and Noble Silence protocols.

---

**👤 You:**
> "What will the silence policy be for a gentle Zen retreat for a beginner?"

**🤖 AI Agent:**
> For a gentle Zen retreat for a beginner, the policy will be Partial Noble Silence, allowing for basic communication during specific windows.

---

**👤 You:**
> "Is a 10-day intensive retreat safe for a beginner?"

**🤖 AI Agent:**
> No, a 10-day intensive retreat is flagged as high risk for a beginner. It is recommended to start with a gentle retreat first.


## ❓ FAQ

**Q: How do I generate a full schedule?**
You can use the `get_retreat_schedule` tool by providing the duration in days, the tradition type, and the desired intensity.

**Q: Can I check if a retreat is too intense for me?**
Yes, use the `validate_retreat_feasibility` tool to check if your planned duration and intensity are suitable for your experience level.

**Q: What information is needed for the daily rhythm?**
To see the breakdown of hours using `calculate_daily_rhythm`, you need to specify the tradition, intensity, and experience level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meditation-retreat-planner](https://vinkius.com/en/ai-agent-connect/meditation-retreat-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meditation Retreat Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meditation-retreat-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meditation Retreat Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meditation-retreat-planner": {
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
