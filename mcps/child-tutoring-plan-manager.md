# Child Tutoring Plan Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/child-tutoring-plan-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage academic subjects, tutor sessions, homework, and budgets in one place.

## Description
This MCP server provides a complete management system for academic tutoring. It allows AI agents to organize academic subjects, schedule tutor sessions using `schedule_tutor_session`, manage homework assignments with `manage_homework`, track student mastery via `track_progress`, and monitor financial health through `audit_budget`. It is designed to keep tutoring plans organized, on schedule, and within budget.


## Available Tools (5)
- **audit_budget**: Provides a financial health report of the tutoring plan
- **get_subject_overview**: Provides a high-level summary of all academic subjects currently in the plan
- **manage_homework**: Creates or updates homework assignments for a specific subject
- **schedule_tutor_session**: Books a specific time for a tutor to meet with the student
- **track_progress**: Logs a progress checkpoint to evaluate student mastery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Child Tutoring Plan Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me an overview of all my current subjects."

**🤖 AI Agent:**
> You are currently tracking Mathematics (85% progress, 2 active homeworks) and Science (40% progress, 1 active homework).

---

**👤 You:**
> "Schedule a Math session with Tutor Sarah for tomorrow from 2 PM to 3 PM at $40 per hour."

**🤖 AI Agent:**
> The Math session with Sarah has been successfully scheduled for tomorrow.

---

**👤 You:**
> "I finished my Science homework. Can you mark it as complete?"

**🤖 AI Agent:**
> The Science homework assignment has been updated to completed.


## ❓ FAQ

**Q: How do I check if I have enough money left for more sessions?**
You can use the `audit_budget` tool to get a financial health report, including remaining funds and projected spending.

**Q: Can I schedule multiple subjects at once?**
Yes, you can use `schedule_tutor_session` for any subject defined in your plan to book specific time slots.

**Q: How is student progress recorded?**
Progress is recorded using the `track_progress` tool, which logs scores and qualitative notes to update the subject's mastery percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/child-tutoring-plan-manager](https://vinkius.com/en/ai-agent-connect/child-tutoring-plan-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Child Tutoring Plan Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `child-tutoring-plan-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Child Tutoring Plan Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "child-tutoring-plan-manager": {
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
