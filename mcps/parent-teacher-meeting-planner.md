# Parent-Teacher Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/parent-teacher-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes meeting schedules by reconciling time constraints, topic priorities, and language needs.

## Description
This MCP server acts as an intelligent orchestration engine for school communications. It helps administrators and parents organize efficient meetings by managing meeting slots, parent availability, and topic priorities. Use `create_attendance_plan` to match participants to available windows, `generate_meeting_agenda` to build structured timelines, `generate_question_list` to prepare parents with targeted questions, and `create_action_record_template` to ensure organized follow-ups following the One-Note-Owner rule.


## Available Tools (4)
- **create_action_record_template**: Generates a standardized document for recording decisions and tasks during the meeting
- **create_attendance_plan**: Determines which parents and teachers should attend which slots based on availability and requirements
- **generate_meeting_agenda**: Creates a structured timeline for an individual meeting
- **generate_question_list**: Produces a list of targeted questions for parents to ask based on previous notes and topic priorities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parent-Teacher Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 30-minute agenda for meeting ID 123 with topics: Math (High) and Reading (Low)."

**🤖 AI Agent:**
> The agenda for meeting 123 is: 0:00-0:20 Math, 0:20-0:30 Reading. Total time used: 30 minutes.

---

**👤 You:**
> "Generate questions for a parent based on these notes: 'Student struggles with fractions' and priority: Fractions (High)."

**🤖 AI Agent:**
> How can we support the student's understanding of fractions at home? What specific fraction concepts are causing the most difficulty?

---

**👤 You:**
> "Create an action record template for meeting 456 with note owner ID 'teacher_01' and email follow-up."

**🤖 AI Agent:**
> Template created for meeting 456. Note owner: teacher_01. Follow-up method: email. Sections: Decisions, Action Items, and Follow-up instructions.


## ❓ FAQ

**Q: How does the tool handle conflicting schedules?**
The `create_attendance_plan` tool identifies valid overlaps between available meeting slots and parent availability, flagging any unmatched participants.

**Q: Can I ensure critical topics are discussed?**
Yes, by using `generate_meeting_agenda`, higher priority topics are scheduled first to ensure they are addressed within the allotted time.

**Q: What is the One-Note-Owner rule?**
It is a rule enforced by `create_action_record_template` to ensure exactly one person is responsible for recording notes, preventing administrative confusion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/parent-teacher-meeting-planner](https://vinkius.com/en/ai-agent-connect/parent-teacher-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parent-Teacher Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parent-teacher-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parent-Teacher Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parent-teacher-meeting-planner": {
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
