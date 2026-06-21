# Evolio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evolio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Transform your coaching practice with client tracking, session management, and progress analytics that help people grow.

## Description
Connect your **Evolio** account to any AI agent and manage your law firm operations through natural conversation.

### What you can do

- **Case Management** — Create, update, list, and inspect cases with status, assigned attorneys, deadlines, and milestones
- **Status Filtering** — Filter cases by status (active, pending, closed, archived) to focus on what needs attention
- **Task Tracking** — Create tasks linked to cases, list all tasks with due dates and assignees, and inspect individual task details
- **Client Profiles** — Browse all clients with contact information and associated case counts, and inspect full client profiles
- **Document Access** — List all documents uploaded per client or per case for easy reference during consultations

### How it works

1. Subscribe to this server
2. Enter your Evolio API Key from your administration settings
3. Start managing your cases from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Attorneys** — check case status, review deadlines, and create tasks without switching to the Evolio dashboard
- **Paralegals** — access client documents and case files during research through conversational AI
- **Law Firm Administrators** — monitor caseloads, track pending tasks, and manage client profiles


## Available Tools (14)
- **check_evolio_status**: Verify connectivity
- **create_case**: Create a case
- **create_task**: Create a task
- **get_case**: Get case details
- **get_client**: Get client details
- **get_task**: Get task details
- **list_cases_by_status**: List cases by status
- **list_case_files**: List case files
- **list_cases**: List cases
- **list_client_files**: List client files
- **list_clients**: List clients
- **list_tasks_by_case**: List tasks by case
- **list_tasks**: List all tasks
- **update_case**: Update a case


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evolio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all active cases and the pending tasks for the one with the nearest deadline."

**🤖 AI Agent:**
> Found 12 active cases. The nearest deadline is case 'Silva Immigration Petition' (case_4012, attorney: Dr. Kovář). Deadline: May 2, 2025 (6 days remaining). This case has 4 pending tasks: 1) 'Submit I-140 form' (due May 1, assigned: Jana). 2) 'Gather supporting documents' (due Apr 30, assigned: Tomáš). 3) 'Client interview prep' (due Apr 29, assigned: Dr. Kovář). 4) 'Translation verification' (due May 2, assigned: External). Would you like to create a new task or update the case status?

---

**👤 You:**
> "List all documents for client Maria Santos and the files attached to her residence permit case."

**🤖 AI Agent:**
> Client 'Maria Santos' (client_891) has 8 uploaded documents: passport scan, birth certificate (translated), employment contract, bank statements (3 months), university diploma, criminal record clearance, health insurance card, and photo ID. Her residence permit case (case_3987) has 5 linked files: application form (PDF), cover letter (DOCX), evidence bundle (PDF, 42 pages), embassy correspondence (PDF), and fee payment receipt. Would you like to review the case details or check task progress?

---

**👤 You:**
> "Create a new family law case for client Jan Novák and add a task to file the initial petition by next Friday."

**🤖 AI Agent:**
> Case created! ID: case_4028, Client: Jan Novák (client_234), Type: Family Law, Status: active, Assigned attorney: Dr. Procházková. Task created! ID: task_8901, Title: 'File initial petition', Due: May 2, 2025 (Friday), Assigned: Dr. Procházková, Linked case: case_4028. The case now appears in the active cases list. Would you like to add more tasks or upload documents?


## ❓ FAQ

**Q: Can I create new cases and tasks directly through the AI agent?**
Yes! The `create_case` action accepts a JSON payload with client, case type, and initial status. The `create_task` action creates tasks linked to specific cases with description, due date, and assignee. Use `update_case` to modify case status, notes, or attorney assignments as the case progresses.

**Q: Can I filter cases by their current status?**
Yes. The `list_cases_by_status` tool accepts a status parameter — 'active', 'pending', 'closed', or 'archived'. This lets you quickly focus on active matters requiring attention, review pending cases awaiting decisions, or audit closed cases for reporting.

**Q: Can I access client documents and case files through the AI agent?**
Yes. Use `list_client_files` with a Client ID to retrieve all documents uploaded for that client. Use `list_case_files` with a Case ID to see all documents associated with a specific case. Both tools return file names, upload dates, and file types for easy reference.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evolio](https://vinkius.com/mcp/evolio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evolio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `evolio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evolio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evolio": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
