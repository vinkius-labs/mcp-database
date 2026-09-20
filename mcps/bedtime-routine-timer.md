# Bedtime Routine Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bedtime-routine-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Reverse-engineer your perfect bedtime routine using sleep hygiene principles.

## Description
This MCP server helps you structure a healthy sleep schedule by calculating optimal start times and activity sequences. Using proven sleep hygiene principles, it determines your `screen_cutoff_time` and organizes activities to maximize relaxation. You can use `calculate_routine_schedule` to generate a full itinerary, `optimize_activity_sequence` to prioritize relaxing tasks, and `evaluate_screen_hygiene` to identify the best time to put away devices. It is designed to help you transition from daily activity to sleep readiness effectively.


## Available Tools (4)
- **calculate_routine_schedule**: Generates a complete, time-sequenced itinerary for a bedtime routine
- **evaluate_screen_hygiene**: Determines the safest time to stop using electronic devices based on user habits
- **get_routine_readiness_score**: Provides a qualitative assessment of how well a proposed routine aligns with sleep hygiene standards
- **optimize_activity_sequence**: Reorders a set of activities to maximize sleep quality based on relaxation needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bedtime Routine Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to be asleep by 22:30. My activities are reading for 20 minutes and stretching for 15 minutes. Can you make a schedule?"

**🤖 AI Agent:**
> To be asleep by 22:30, your routine should start at 21:55. Your sequence is: Stretching (21:55 - 22:10) followed by Reading (22:10 - 22:30).

---

**👤 You:**
> "I use my phone a lot before bed. When should I stop using it if I want to sleep at 23:00?"

**🤖 AI Agent:**
> Based on your high device usage, you should stop using electronic devices at 22:00 to ensure a healthy transition to sleep.

---

**👤 You:**
> "Help me organize these activities for maximum relaxation: brushing teeth (5 min), meditation (15 min), and light reading (20 min). I want to sleep at 22:00."

**🤖 AI Agent:**
> To maximize relaxation, your optimized sequence is: Brushing teeth (21:20 - 21:25), Light reading (21:25 - 21:45), and Meditation (21:45 - 22:00).


## ❓ FAQ

**Q: How does the routine calculation work?**
The tool works backward from your desired sleep time to determine when you should start your routine and when you must stop using electronic devices.

**Q: Can I prioritize relaxing activities?**
Yes, you can use the `optimize_activity_sequence` tool to reorder your tasks so that the most relaxing ones occur closest to your sleep time.

**Q: What is screen cutoff?**
Screen cutoff is the specific time when you should stop using all electronic devices to allow your body to prepare for sleep without blue light interference.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bedtime-routine-timer](https://vinkius.com/en/ai-agent-connect/bedtime-routine-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bedtime Routine Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bedtime-routine-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bedtime Routine Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bedtime-routine-timer": {
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
