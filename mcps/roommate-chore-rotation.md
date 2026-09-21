# Roommate Chore Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/roommate-chore-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Distribute household chores equitably using effort points and roommate weights.

## Description
This MCP server automates fair household chore scheduling. It uses effort points to quantify task difficulty and roommate weights to adjust for individual capacities. You can use `generate_weekly_schedule` to create a balanced weekly plan, `calculate_effort_distribution` to determine target workloads, `find_uncovered_tasks` to identify scheduling gaps, and `validate_schedule_fairness` to audit the distribution.


## Available Tools (4)
- **calculate_effort_distribution**: Determines the theoretical target effort each roommate should handle to achieve balance
- **find_uncovered_tasks**: Identifies which tasks could not be assigned to any roommate due to constraints
- **generate_weekly_schedule**: Produces a complete, optimized schedule of tasks for a one-week period
- **validate_schedule_fairness**: Audits a generated schedule to ensure it adheres to the effort-balancing logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roommate Chore Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a weekly chore schedule for my roommates."

**🤖 AI Agent:**
> Here is the optimized weekly schedule: Monday: Dishes (Alice, 2pts), Tuesday: Vacuuming (Bob, 3pts), Wednesday: Trash (Alice, 1pt)...

---

**👤 You:**
> "How much effort should each roommate handle?"

**🤖 AI Agent:**
> Based on the provided weights, the target effort distribution is: Alice: 15pts, Bob: 10pts, Charlie: 15pts.

---

**👤 You:**
> "Check if the current schedule is fair."

**🤖 AI Agent:**
> The schedule is fair. The deviation from target effort for all roommates is within the acceptable range.


## ❓ FAQ

**Q: How is fairness determined?**
Fairness is achieved by balancing the ratio of actual effort points assigned to a person against their specific roommate weight.

**Q: Can I handle tasks I am excluded from?**
No, the system respects exclusion constraints to ensure no roommate is assigned a task they are barred from performing.

**Q: What happens if a task cannot be assigned?**
If a task cannot be assigned due to availability or exclusion constraints, you can use `find_uncovered_tasks` to identify it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/roommate-chore-rotation](https://vinkius.com/en/ai-agent-connect/roommate-chore-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roommate Chore Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roommate-chore-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roommate Chore Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roommate-chore-rotation": {
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
