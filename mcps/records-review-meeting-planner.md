# Records Review Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/records-review-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms household administrative data into structured meeting agendas and action plans.

## Description
This MCP server automates household governance by converting administrative data into actionable meeting plans. It applies strict rules like the Fixed Agenda Rule and Evidence-Closure to ensure all record changes and expirations are addressed. Use `generate_meeting_agenda` to build your schedule, `verify_category_ownership` to confirm authorized reviewers, `create_action_plan` to assign tasks, and `calculate_next_review` to schedule your next session.


## Available Tools (4)
- **calculate_next_review**: If the expiringItemCount is greater than 3, the interval is reduced to 3 months.

Determines when the household should meet again
- **create_action_plan**: Assignments can only be made to names provided in the participants list.

Generates the list of tasks and assignments required to close out pending issues
- **generate_meeting_agenda**: The agenda must include specific line items for every provided "recent change" and "expiring item".

Creates the structured schedule for the meeting based on the provided household context
- **verify_category_ownership**: Validates that the people present are authorized to review the requested categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Records Review Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a meeting agenda for Alice and Bob on 2024-05-01 for Medical and Financial records, noting a new insurance policy and an expiring passport."

**🤖 AI Agent:**
> Meeting Agenda for 2024-05-01:
1. Participant Confirmation: Alice, Bob
2. Category Review:
   - Medical: Review new insurance policy
   - Financial: Review expiring passport
3. Security Audit
4. Action Assignment

---

**👤 You:**
> "Who is authorized to review the Medical category if Alice and Bob are present and Alice is the owner?"

**🤖 AI Agent:**
> Alice is authorized to review the Medical category.

---

**👤 You:**
> "When should the next meeting be if there are 4 expiring items today, 2024-01-01?"

**🤖 AI Agent:**
> The next meeting is scheduled for 2024-04-01.


## ❓ FAQ

**Q: How does the agenda generation work?**
The `generate_meeting_agenda` tool follows a fixed sequence: Participant Confirmation, Category Review, Security Audit, and Action Assignment.

**Q: What happens if a category owner is missing?**
The `verify_category_ownership` tool will identify the category as invalid if the designated owner is not in the participant list.

**Q: How are tasks assigned?**
The `create_action_plan` tool ensures every recent change or expiring item results in a specific assignment to a participant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/records-review-meeting-planner](https://vinkius.com/en/ai-agent-connect/records-review-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Records Review Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `records-review-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Records Review Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "records-review-meeting-planner": {
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
