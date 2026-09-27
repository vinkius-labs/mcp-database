# Repair Communication Log Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-communication-log-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured communication schedules, message templates, and escalation workflows.

## Description
This MCP server provides a professional toolset for managing project communications. It allows AI agents to generate comprehensive communication strategies, including templates, calendars, and next-contact queues. By applying a fixed update cadence and an automated escalation ladder, it ensures stakeholders are informed according to their influence and interest levels. Use `generate_communication_plan` to build the strategy, `calculate_next_contacts` to prioritize upcoming tasks, `get_message_templates` for drafted messages, and `log_decision` to maintain a formal audit trail.


## Available Tools (4)
- **calculate_next_contacts**: Generates a prioritized list of the very next communications that need to happen
- **get_message_templates**: Retrieves formatted message drafts based on the specific communication event
- **log_decision**: Records a formal decision into the project's decision log
- **generate_communication_plan**: Creates a comprehensive communication strategy including templates, calendars, and queues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Communication Log Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a communication plan for a 3-month construction project with high-influence stakeholders."

**🤖 AI Agent:**
> The communication plan has been generated. It includes a weekly update cadence for Tier 1 stakeholders and a monthly summary for Tier 3 stakeholders.

---

**👤 You:**
> "What are my next scheduled contacts for this week?"

**🤖 AI Agent:**
> Your next contacts are: 1. Project Sponsor (Email, High Priority), 2. Technical Lead (Slack, Medium Priority).

---

**👤 You:**
> "Draft an escalation message for a missed deadline with the Executive stakeholder."

**🤖 AI Agent:**
> Subject: Urgent: Missed Response Deadline - Project Update. Dear Executive, this is a formal notification regarding the missed deadline for the recent project milestone.


## ❓ FAQ

**Q: How do I create a new communication strategy?**
You can use the `generate_communication_plan` tool by providing stakeholder details, project phases, and notice requirements as JSON strings.

**Q: What happens if a response deadline is missed?**
The system automatically triggers the escalation ladder, moving communication to higher-level stakeholders or more formal channels.

**Q: Can I record project decisions?**
Yes, use the `log_decision` tool to record formal decisions and maintain a clear audit trail for the project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-communication-log-plan](https://vinkius.com/en/ai-agent-connect/repair-communication-log-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Communication Log Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-communication-log-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Communication Log Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-communication-log-plan": {
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
