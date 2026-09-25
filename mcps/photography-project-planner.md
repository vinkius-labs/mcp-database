# Photography Project Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photography-project-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic planning engine for photography projects, generating briefs, logistics, and workflows.

## Description
This MCP server transforms raw photography parameters into structured strategic documents. It provides tools to `plan_project_brief` for core strategy, `calculate_shoot_commitments` for logistics and timelines, `generate_permission_checklist` for legal and consent requirements, and `map_workflow_milestones` to define collaborator handoffs and quality checkpoints. It acts as a bridge between creative vision and logistical execution.

### Available Tools

`plan_project_brief_tool`, `calculate_shoot_commitments_tool`, `generate_permission_checklist_tool`, `map_workflow_milestones_tool`


## Available Tools (4)
- **calculate_shoot_commitments_tool**: 
- **generate_permission_checklist_tool**: 
- **map_workflow_milestones_tool**: 
- **plan_project_brief_tool**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photography Project Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a high-fashion shoot in a desert with two models for a magazine cover."

**🤖 AI Agent:**
> The strategic brief for your high-fashion desert shoot focuses on dramatic lighting and expansive compositions to suit the magazine cover format. Constraints include managing heat and limited daylight windows.

---

**👤 You:**
> "Calculate the logistics for a city street shoot ending on Friday."

**🤖 AI Agent:**
> The logistics schedule accounts for transit between urban locations and ensures all setup is completed before the Friday deadline.

---

**👤 You:**
> "Map the workflow for a team consisting of a Photographer, Stylist, and Assistant."

**🤖 AI Agent:**
> The workflow includes handoffs from the Stylist to the Photographer for setup, and specific review checkpoints to ensure the visual direction is met before final output.


## ❓ FAQ

**Q: What can this MCP server do?**
It automates the creation of photography project briefs, calculates logistical commitments like schedules, generates permission checklists for locations and models, and maps out workflow milestones. Tools available: `plan_project_brief_tool`, `calculate_shoot_commitments_tool`, `generate_permission_checklist_tool`.

**Q: How do I use the planning tool?**
You can use the `plan_project_brief` tool by providing the theme, subjects, and intended output to generate a cohesive strategic guide.

**Q: Does it handle legal permissions?**
Yes, the `generate_permission_checklist` tool identifies necessary legal and consent-based actions based on your participants and locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photography-project-planner](https://vinkius.com/en/ai-agent-connect/photography-project-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photography Project Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photography-project-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photography Project Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photography-project-planner": {
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
