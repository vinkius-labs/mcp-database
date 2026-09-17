# Exercise Max Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/exercise-max-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track lifting progress, estimated 1RM, and strength trends.

## Description
Manage your strength progression by recording lifting sessions and analyzing performance. This MCP allows you to use `log_lift_session` to record weight and reps, `get_current_max` to find your latest estimated 1RM, and `get_strength_trend` to see if your strength is improving over time. You can also evaluate your `get_relative_strength_metrics` to see how your strength compares to your body weight.


## Available Tools (5)
- **get_current_max**: Retrieves the most recent estimated 1RM for a specific exercise
- **compare_performance_periods**: Compares current strength performance against a previous timeframe
- **get_relative_strength_metrics**: Calculates how strong the lifter is relative to their own body weight for a specific exercise
- **get_strength_trend**: Analyzes the trajectory of strength for an exercise over a specified duration
- **log_lift_session**: Records a single lifting set to the database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exercise Max Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just did 100kg for 5 reps on Bench Press today. My body weight is 85kg."

**🤖 AI Agent:**
> I have recorded your Bench Press session: 100kg for 5 reps at a body weight of 85kg.

---

**👤 You:**
> "What is my current max for Squat?"

**🤖 AI Agent:**
> Your current estimated 1RM for Squat is 145kg, based on your last session.

---

**👤 You:**
> "How has my strength trended for Deadlift over the last 30 days?"

**🤖 AI Agent:**
> Your Deadlift strength has improved by 5% over the last 30 days.


## ❓ FAQ

**Q: How do I record a new lift?**
Use the `log_lift_session` tool by providing the exercise name, weight, repetitions, your body weight, and the date.

**Q: How is my 1RM calculated?**
The system estimates your one-repetition maximum based on the weight and repetitions recorded in your sessions.

**Q: Can I see my strength progress over time?**
Yes, you can use `get_strength_trend` to analyze your strength trajectory over a specific number of days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/exercise-max-tracker](https://vinkius.com/en/ai-agent-connect/exercise-max-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exercise Max Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exercise-max-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exercise Max Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exercise-max-tracker": {
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
