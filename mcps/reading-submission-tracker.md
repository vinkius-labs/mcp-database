# Reading Submission Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reading-submission-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage manuscript submission timelines and follow-up schedules.

## Description
This MCP server provides tools to manage the lifecycle of academic or literary manuscript submissions. It allows users to monitor submission dates, track response windows, and identify when a follow-up is required. Use `list_all_submissions` to view the full tracker, `get_overdue_responses` to find missed deadlines, `get_due_follow_ups` to identify manuscripts needing immediate contact, and `update_submission_status` to transition manuscripts through stages like Pending, Followed Up, or Decided.


## Available Tools (4)
- **get_overdue_responses**: Identifies manuscripts that have missed their expected response deadline but are not yet at the stage where a follow-up is recommended
- **list_all_submissions**: Retrieves a complete list of all manuscripts currently in the tracker
- **update_submission_status**: Updates the lifecycle stage of a specific manuscript
- **get_due_follow_ups**: Identifies manuscripts that require immediate action via a follow-up communication


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reading Submission Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the manuscripts I am currently tracking."

**🤖 AI Agent:**
> Here are your current manuscript submissions: [Manuscript ID: MS-101, Date: 2023-10-01, Status: Pending; Manuscript ID: MS-102, Date: 2023-09-15, Status: Followed Up]

---

**👤 You:**
> "Which submissions are overdue for a response?"

**🤖 AI Agent:**
> The following manuscripts have missed their expected response deadline: [Manuscript ID: MS-105, Expected Date: 2023-10-10, Status: Pending]

---

**👤 You:**
> "Mark manuscript MS-202 as Decided."

**🤖 AI Agent:**
> Manuscript MS-202 has been successfully updated to Decided.


## ❓ FAQ

**Q: How do I see all my tracked manuscripts?**
You can use the `list_all_submissions` tool to retrieve a complete list of all manuscripts currently in the tracker.

**Q: How can I identify manuscripts that need a follow-up?**
Use the `get_due_follow_ups` tool to find manuscripts that have passed both their response window and their required follow-up interval.

**Q: Can I change the status of a submission?**
Yes, you can use `update_submission_status` to move a manuscript to states such as Followed Up or Decided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reading-submission-tracker](https://vinkius.com/en/ai-agent-connect/reading-submission-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reading Submission Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reading-submission-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reading Submission Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reading-submission-tracker": {
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
