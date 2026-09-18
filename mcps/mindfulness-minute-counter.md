# Mindfulness Minute Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mindfulness-minute-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and project your mindfulness practice progress and habit growth.

## Description
This MCP server provides tools to monitor mindfulness habits through detailed metrics. Use `get_practice_summary` to see your total time and current streaks, or `get_streak_metrics` to analyze your consistency and momentum. You can also use `get_annual_projection` to estimate future practice volume or `get_milestone_progress` to track how close you are to your next mindfulness goal.


## Available Tools (4)
- **get_practice_summary**: Provides a summary of total practice time and current streak status
- **get_annual_projection**: Predicts future practice volume based on current habit strength
- **get_milestone_progress**: Identifies how close the user is to significant achievement markers
- **get_streak_metrics**: Provides deep dive metrics into streak quality and consistency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mindfulness Minute Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total time have I spent meditating and what is my current streak?"

**🤖 AI Agent:**
> You have practiced for a total of 450 minutes over 15 days, and your current streak is 5 days.

---

**👤 You:**
> "How close am I to my 500-minute milestone?"

**🤖 AI Agent:**
> You have achieved 450 minutes. Your next milestone is 500 minutes, and you are 90% of the way there.

---

**👤 You:**
> "What is my projected practice for the year based on my current momentum?"

**🤖 AI Agent:**
> Based on your current habit strength, you are projected to practice for 2,500 minutes over 200 active days this year.


## ❓ FAQ

**Q: How do I calculate my current streak?**
You can use the `get_practice_summary` tool to retrieve your current consecutive days of practice based on your daily minutes history.

**Q: Can I predict my future meditation time?**
Yes, the `get_annual_projection` tool uses your current habit momentum and historical averages to estimate your total minutes for a full year.

**Q: How are milestones determined?**
By using `get_milestone_progress`, you can provide specific minute targets to see your progress and identify your next achievement marker.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mindfulness-minute-counter](https://vinkius.com/en/ai-agent-connect/mindfulness-minute-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mindfulness Minute Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mindfulness-minute-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mindfulness Minute Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mindfulness-minute-counter": {
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
