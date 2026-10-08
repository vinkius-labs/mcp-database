# Hobby-Relaxation-Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hobby-relaxation-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Protects personal well-being by scheduling hobby time around mandatory household duties.

## Description
The Hobby-Relaxation-Scheduler is a time-management system that treats personal hobbies as non-negotiable wellness requirements. By using `get_weekly_availability` and `get_household_obligations`, the system identifies free time blocks. It then uses `calculate_relaxation_capacity` to determine the actual available minutes and `schedule_hobby_projects` to fit your specific activities into those windows. This ensures you meet your minimum relaxation target and avoid a relaxation deficit.


## Available Tools (4)
- **calculate_relaxation_capacity**: Determines how much actual free time remains after household duties
- **get_household_obligations**: Retrieves all mandatory household duties
- **get_weekly_availability**: Retrieves all available time windows for the week
- **schedule_hobby_projects**: Attempts to fit specific hobby projects into the remaining free time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hobby-Relaxation-Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my available time for hobbies this week."

**🤖 AI Agent:**
> You have 420 minutes of free time available across three windows this week after accounting for your household duties.

---

**👤 You:**
> "Schedule my painting and reading projects with a 120 minute relaxation target."

**🤖 AI Agent:**
> I have scheduled Painting for Tuesday from 2:00 PM to 3:30 PM and Reading for Thursday from 4:00 PM to 5:00 PM. Your relaxation target has been met.

---

**👤 You:**
> "How much free time do I have left after my chores?"

**🤖 AI Agent:**
> After subtracting your mandatory household duties, you have 350 minutes of remaining free time available for hobbies.


## ❓ FAQ

**Q: How does the scheduler handle household duties?**
Household duties are treated as hard constraints. The system uses `get_household_obligations` to identify these fixed blocks and subtracts them from your available windows before scheduling any hobbies.

**Q: What happens if I don't meet my relaxation target?**
If the scheduled hobby durations are less than your minimum target, the system reports a relaxation deficit, indicating how many minutes you fell short of your wellness goal.

**Q: Can I schedule projects that are longer than my free time blocks?**
No. A hobby project can only be scheduled if its full duration fits within a single continuous free block identified by `calculate_relaxation_capacity`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hobby-relaxation-scheduler](https://vinkius.com/en/ai-agent-connect/hobby-relaxation-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hobby-Relaxation-Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hobby-relaxation-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hobby-Relaxation-Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hobby-relaxation-scheduler": {
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
