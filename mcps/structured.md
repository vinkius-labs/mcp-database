# Structured MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/structured)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI to Structured. Programmatically manage your daily planner, tasks, and routines seamlessly directly from your terminal.

## Description
Integrate the powerful tracking of the **Structured** daily planner directly into your conversational AI environment. Empower your productivity by allowing your LLM to intuitively create tasks, schedule complex recurring routines, and manage your day programmatically without opening the mobile app. With this MCP connector securely attached to your Structured Pro environment, your agent can serve as an active scheduling assistant, iterating dynamically through your agenda, parsing task structures, and executing adjustments organically.

### What you can do

- **Agenda Discovery** — Audit your scheduled events querying active records using `list_tasks` and retrieve deep metadata specific assignments utilizing `get_task_details`.
- **Task Orchestration** — Drive agile agenda resolutions adding new items seamlessly executing `create_task` or adjusting timelines using `update_task`.
- **Routine Management** — Check your active multi-step routines effectively through `list_plans` and isolate their specific structural constraints engaging `get_plan_details`.
- **Profile Validations** — Safely extract your user metadata boundaries and operational statuses natively invoking `get_user_profile`.

### How it works

1. Enable the Structured MCP module configuring it logically as an active integration.
2. In the parameter matrix, bind your official `STRUCTURED_TOKEN` (provided effectively via Structured Pro settings).
3. State your objective: "Assess my planned tasks for today, generate a new activity block for 'System Architecture Review', and organize it dynamically."

### Who is this for?

- **Founders & Executives** — Manage aggressive schedules completely iteratively without breaking focus, simply dictating adjustments naturally via your AI agent.
- **Independent Creators** — Monitor creative blocks, formulate specific routines, and execute tasks dynamically interacting transparently with your daily tracking tool.
- **Software Engineers** — Bind your daily agenda directly into your IDE conversational AI securely tracking progress locally.


## Available Tools (9)
- **list_plans**: Lists all structured plans
- **get_plan_details**: Retrieves details for a specific plan
- **create_plan**: Creates a new plan
- **get_user_profile**: Retrieves the current user profile
- **list_tasks**: Lists all tasks in Structured
- **get_task_details**: Retrieves details for a specific task
- **create_task**: Provide a title and optional start time.

Creates a new task in Structured
- **update_task**: Updates an existing task
- **delete_task**: This action is irreversible.

Permanently deletes a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Structured** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assess my active Structured environment, listing today's pending tasks, and mark the scheduled meeting block as successfully completed."

**🤖 AI Agent:**
> Validating parameters seamlessly...
**Current Pending Tasks Mapped (`list_tasks`)**:
- `Code Architecture Assessment`
- `Managerial Meeting`

Updating attribute structurally calling task parameter natively:
- Task `Managerial Meeting` has been updated cleanly. `isCompleted` now reflects successfully finalized metric natively explicitly effectively correctly.
Ready to process subsequent routine deployments actively.

---

**👤 You:**
> "List all active plans for the week, and display the detailed constraints of the 'Morning Focus' routine."

**🤖 AI Agent:**
> Retrieving your routine logic matrices seamlessly...
**Routines Acquired (`list_plans`)**:
- `Morning Focus`
- `Evening Winding Down`

Deep inspecting context using `get_plan_details` natively...
The 'Morning Focus' demands 90 uninterrupted minutes without communication applications.

---

**👤 You:**
> "Read my user profile cleanly to extract my workspace validation level and operational timezone."

**🤖 AI Agent:**
> Auditing operational attributes accurately...
Executing `get_user_profile` locally natively successfully.
**Authentication Response**:
- User Authorization: `Structured Pro` active successfully.
- Locale Definition: `Europe/London` applied proactively.
The context is perfectly mapped.


## ❓ FAQ

**Q: Do I need a paid plan to use the Structured programmatic API?**
Yes. Programmatic integrations and the ability to systematically generate and query your personal API access require a Structured Pro plan to safely extract the required access tokens securely.

**Q: Can the integration delete past records destructively by accident executing commands natively?**
Risk is inherently mitigated. The AI only calls mutations like `delete_task` precisely when instructed unequivocally. Records aren't inherently purged on exploration, allowing safe queries comprehensively continuously naturally.

**Q: Which platforms does the Structured integration support?**
The MCP connects to the Structured Pro API, which syncs across iOS, iPadOS, macOS, and the web app. Any task created or updated via the AI is reflected on all your devices in real time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/structured](https://vinkius.com/mcp/structured)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Structured** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `structured` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Structured** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "structured": {
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
