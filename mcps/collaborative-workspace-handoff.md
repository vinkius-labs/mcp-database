# Collaborative Workspace Handoff MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/collaborative-workspace-handoff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate structured digital workspace migrations with staged checklists.

## Description
This MCP server provides a complete framework for managing the transition of digital workspaces. It allows AI agents to orchestrate ownership transfers, audit member permissions, identify successor roles, and generate sequenced, staged checklists to ensure a smooth migration. Use `get_workspace_summary` to assess the current state, `audit_access_permissions` to identify security gaps, `list_successor_roles` to prepare for continuity, and `generate_handoff_checklist` to drive the migration process through its required stages: Role Succession, Permission Audit, File/Asset Transfer, and Final Ownership Shift.


## Available Tools (4)
- **generate_handoff_checklist**: Produces a sequenced, staged checklist of tasks required to complete the ownership transfer
- **list_successor_roles**: Identifies all individuals currently designated as successors for key roles within the workspace
- **audit_access_permissions**: Evaluates current access restrictions and identifies potential security gaps during a transition
- **get_workspace_summary**: Provides a high-level overview of the current state of a specific workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collaborative Workspace Handoff** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the workspace with ID 'ws-123'."

**🤖 AI Agent:**
> The workspace 'ws-123' is currently owned by Alice, has 5 members, 12 files, and the transfer status is pending.

---

**👤 You:**
> "Who are the successors for the current roles in workspace 'ws-456'?"

**🤖 AI Agent:**
> The designated successors for workspace 'ws-456' are Bob (Manager, readiness 0.9) and Charlie (Contributor, readiness 0.7).

---

**👤 You:**
> "Generate a handoff checklist for workspace 'ws-789' for the date 2025-12-01."

**🤖 AI Agent:**
> The handoff checklist for 'ws-789' has been generated. The current completion is 0%. Stages include Role Succession, Permission Audit, File/Asset Transfer, and Final Ownership Shift.


## ❓ FAQ

**Q: How do I start a workspace migration?**
You can begin by using `get_workspace_summary` to understand the current state of the workspace and then call `generate_handoff_checklist` to receive the required sequence of tasks.

**Q: Can I audit security during the handoff?**
Yes, the `audit_access_permissions` tool allows you to evaluate access restrictions and identify potential security conflicts during the transition.

**Q: What are the stages of the handoff checklist?**
The checklist follows a strict sequence: 1. Role Succession, 2. Permission Audit, 3. File/Asset Transfer, and 4. Final Ownership Shift.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/collaborative-workspace-handoff](https://vinkius.com/en/ai-agent-connect/collaborative-workspace-handoff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collaborative Workspace Handoff** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `collaborative-workspace-handoff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collaborative Workspace Handoff** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collaborative-workspace-handoff": {
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
