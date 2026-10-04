# Academic Writing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/academic-writing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Decomposes essays into structured phases: Outline, Research, Drafting, Editing, and Submission.

## Description
This MCP server manages the full lifecycle of academic writing. It breaks down complex essay assignments into manageable tasks across five core phases: Outline, Research, Drafting, Editing, and Submission. Use `create_writing_plan` to generate a custom schedule based on your essay type and deadline, `get_essay_summary` to track overall progress, and `update_task_status` to mark individual tasks as complete. It ensures that research and drafting are balanced according to the specific essay requirements.


## Available Tools (5)
- **get_essay_summary**: Retrieves a high-level overview of a specific essay plan
- **get_phase_details**: Retrieves all tasks and sub-tasks associated with a specific phase of an essay
- **list_all_plans**: Provides a list of all active academic writing plans managed by the user
- **update_task_status**: Marks a specific task within a phase as complete or incomplete
- **create_writing_plan**: Generates a full lifecycle of tasks based on an essay's requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Academic Writing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to write an argumentative essay titled 'The Impact of AI on Education' due on 2025-05-20. Can you create a plan for me?"

**🤖 AI Agent:**
> I have created your writing plan for 'The Impact of AI on Education'. The plan includes phases for Outline, Research, Drafting, Editing, and Submission, all scheduled to be completed by May 20th, 2025.

---

**👤 You:**
> "What is the current status of my essay plan 'Climate Change Analysis'?"

**🤖 AI Agent:**
> Your essay plan 'Climate Change Analysis' is currently in the Research phase. You have completed 40% of the total tasks.

---

**👤 You:**
> "Show me the tasks for the Research phase of my current essay."

**🤖 AI Agent:**
> The Research phase includes: 1. Gather primary sources, 2. Review academic journals, and 3. Organize citations.


## ❓ FAQ

**Q: How do I start a new essay project?**
You can use the `create_writing_plan` tool by providing the essay title, your target deadline, and the essay type (argumentative or analytical).

**Q: Can I track my progress through different phases?**
Yes, you can use `get_essay_summary` to see your current phase and completion percentage, or `get_phase_details` to view specific tasks within a phase.

**Q: How do I mark a task as finished?**
Use the `update_task_status` tool with the specific `essayId` and `taskId` to mark a task as completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/academic-writing-plan](https://vinkius.com/en/ai-agent-connect/academic-writing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Academic Writing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `academic-writing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Academic Writing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "academic-writing-plan": {
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
