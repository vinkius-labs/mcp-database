# Family Responsibility Board MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-responsibility-board)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate household and childcare logistics with structured ownership and rotation logic.

## Description
The Family Responsibility Board connects AI agents to your household logistics. It manages recurring tasks by applying one-primary-owner, backup-owner, and rotation rules. Use `get_responsibility_board` to view current task status and workload distribution, `generate_weekly_assignments` to create upcoming schedules, `get_handoff_instructions` to ensure smooth transitions between owners, and `get_review_points` to identify when to audit fairness or availability.


## Available Tools (4)
- **generate_weekly_assignments**: Generates a specific schedule for the upcoming week based on current rules
- **get_handoff_instructions**: Retrieves the specific operational instructions for a specific person transitioning into a role
- **get_responsibility_board**: Provides a high-level overview of all recurring tasks and their current status
- **get_review_points**: Identifies upcoming dates when the responsibility distribution should be evaluated


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Responsibility Board** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current household task distribution."

**🤖 AI Agent:**
> The current workload is distributed as follows: Alex has 4 tasks, Sam has 3 tasks, and Jordan has 3 tasks.

---

**👤 You:**
> "Generate the schedule for next week starting 2025-05-12."

**🤖 AI Agent:**
> The schedule for the week of 2025-05-12 is ready. Monday: Dishwashing (Alex, Backup: Sam), Tuesday: Trash (Sam, Backup: Jordan), Wednesday: Grocery Shopping (Jordan, Backup: Alex).

---

**👤 You:**
> "What are the instructions for taking over the laundry task on 2025-05-15?"

**🤖 AI Agent:**
> To take over the laundry task, please ensure the dryer is empty and check that the detergent levels are sufficient.


## ❓ FAQ

**Q: How does the rotation logic work?**
The system identifies the next eligible person in the sequence based on their availability and the selected fairness mode, such as equalized or blocked distribution.

**Q: Can I see who is responsible for a task right now?**
Yes, you can use the `get_responsibility_board` tool to see the current primary and backup owners for all registered tasks.

**Q: What happens if a primary owner is unavailable?**
Every task includes a backup owner to ensure coverage. You can use `get_handoff_instructions` to manage the transition when a change in ownership occurs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-responsibility-board](https://vinkius.com/en/ai-agent-connect/family-responsibility-board)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Responsibility Board** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-responsibility-board` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Responsibility Board** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-responsibility-board": {
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
