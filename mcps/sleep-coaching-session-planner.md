# Sleep Coaching Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-coaching-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured coaching agendas, priorities, and homework for sleep professionals.

## Description
This MCP server provides a specialized planning engine for sleep coaches. It transforms client sleep data, goals, and previous interventions into actionable session structures. Coaches can use `get_session_agenda` to create timed meeting flows, `identify_session_priorities` to pinpoint critical issues, `generate_homework` to assign behavioral tasks, and `calculate_progress_summary` to track client improvement over time.


## Available Tools (4)
- **calculate_progress_summary**: Quantifies how much the client has moved toward their goals
- **generate_homework**: Creates actionable behavioral tasks for the client to perform between sessions
- **get_session_agenda**: Generates a timed chronological plan for the coaching session
- **identify_session_priorities**: Determines the most critical sleep issues to address during the meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Coaching Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 30-minute session agenda for a client wanting to improve sleep latency, currently reporting 45 minutes to fall asleep."

**🤖 AI Agent:**
> Here is your 30-minute agenda: 1. Review Progress (5 mins), 2. Goal Alignment (5 mins), 3. Priority Discussion: Sleep Latency (10 mins), 4. Action Planning & Homework (10 mins).

---

**👤 You:**
> "What are the main priorities for a client who has tried reducing caffeine but still struggles with frequent nighttime awakenings?"

**🤖 AI Agent:**
> The primary priority is addressing nighttime awakenings, as previous caffeine reduction did not resolve this specific issue.

---

**👤 You:**
> "Generate homework for a client focused on improving sleep efficiency."

**🤖 AI Agent:**
> Task: Implement a strict wind-down routine 30 minutes before bed. Expected Outcome: Reduced time spent awake in bed and improved sleep efficiency.


## ❓ FAQ

**Q: How does the session agenda generation work?**
The `get_session_agenda` tool uses the provided session duration and client data to create a logical, timed flow from review to action planning.

**Q: Can I track client progress over multiple sessions?**
Yes, by using `calculate_progress_summary`, you can compare current sleep metrics against previous interventions to determine improvement trends.

**Q: How are homework assignments created?**
The `generate_homework` tool creates specific behavioral tasks that are directly mapped to the priorities identified during the session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-coaching-session-planner](https://vinkius.com/en/ai-agent-connect/sleep-coaching-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Coaching Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-coaching-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Coaching Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-coaching-session-planner": {
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
