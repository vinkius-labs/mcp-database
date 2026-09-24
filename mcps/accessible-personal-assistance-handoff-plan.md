# Accessible Personal Assistance Handoff Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-personal-assistance-handoff-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A coordination system for managing personal assistance transitions, task briefings, and safety protocols.

## Description
This MCP server provides a structured framework for managing personal assistance transitions. It enables authorized assistants to receive formal shift handoff protocols, concise task briefings, and change notifications while strictly adhering to user-defined boundaries and consent checkpoints. Use `get_shift_handoff_protocol` for smooth transitions, `get_task_briefing` to review permitted tasks, `get_change_notification` to broadcast routine updates, and `get_unresolved_question_log` to identify safety-critical ambiguities.


## Available Tools (4)
- **get_task_briefing**: Provides a concise summary of specific tasks to be performed, filtered by authorized boundaries
- **get_change_notification**: Creates a formal notification regarding changes in the user's routine or environment
- **get_shift_handoff_protocol**: Generates a formal transition document between outgoing and incoming assistants
- **get_unresolved_question_log**: Retrieves a list of pending questions or ambiguities that must be addressed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Personal Assistance Handoff Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a handoff protocol for the transition between assistant A and assistant B."

**🤖 AI Agent:**
> The transition protocol has been generated. It includes the status of completed tasks, pending items for the incoming assistant, and all active safety checkpoints.

---

**👤 You:**
> "What tasks am I permitted to perform right now?"

**🤖 AI Agent:**
> Your permitted tasks include meal preparation and light housekeeping. Please note the consent trigger for any changes to the user's medication schedule.

---

**👤 You:**
> "Are there any unresolved questions preventing me from starting my shift?"

**🤖 AI Agent:**
> There is one high-priority question regarding the specific location of the user's mobility equipment.


## ❓ FAQ

**Q: How does this server ensure safety during transitions?**
Safety is maintained through `get_shift_handoff_protocol` and `get_task_briefing`, which enforce user-defined consent checkpoints and task boundaries, ensuring no unauthorized actions are taken.

**Q: Can I use this to receive task instructions?**
Yes, assistants can use `get_task_briefing` to receive a summary of permitted tasks and specific consent triggers required for their role.

**Q: What happens if there is a change in the user's routine?**
Changes are managed via `get_change_notification`, which broadcasts updates regarding routine, equipment, or communication to all affected authorized assistants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-personal-assistance-handoff-plan](https://vinkius.com/en/ai-agent-connect/accessible-personal-assistance-handoff-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Personal Assistance Handoff Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-personal-assistance-handoff-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Personal Assistance Handoff Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-personal-assistance-handoff-plan": {
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
