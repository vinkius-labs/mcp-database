# Accessible Workspace Accommodation Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-workspace-accommodation-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured workplace accommodation requests, evidence checklists, and meeting agendas.

## Description
This MCP server provides a structured toolkit for employees to manage workplace accommodation requests. It helps users bridge the gap between identified workplace barriers and requested adjustments by generating formal request briefs, organizing user-identified evidence, and preparing discussion agendas for meetings with decision-makers. Users can also create implementation roadmaps and follow-up communication templates to track their progress through different communication phases.


## Available Tools (5)
- **create_evidence_checklist**: Organize the user's own evidence into a coherent list for verification
- **generate_accommodation_brief**: Create a formal, structured request for a workplace adjustment
- **generate_followup_templates**: Provide ready-to-use text for checking in on the status of an accommodation
- **generate_implementation_plan**: Break down the transition from request to active adjustment into actionable steps
- **prepare_discussion_agenda**: Prepare the user for a meeting with decision-makers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Workspace Accommodation Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to request a standing desk because my current seated setup causes back pain during my coding tasks."

**🤖 AI Agent:**
> I have generated your accommodation request brief. It maps your current back pain during coding tasks to the request for a standing desk, using the provided company ergonomic policy.

---

**👤 You:**
> "Help me organize my medical notes and my recent ergonomic assessment for my accommodation request."

**🤖 AI Agent:**
> I have created your evidence checklist, including your medical notes and the ergonomic assessment, to help you prepare for verification.

---

**👤 You:**
> "I have a meeting with my HR representative tomorrow to discuss my request. I want to ensure I don't share specific medical diagnoses."

**🤖 AI Agent:**
> I have prepared a discussion agenda that focuses on your functional needs and requested adjustments while strictly adhering to your confidentiality boundaries regarding medical diagnoses.


## ❓ FAQ

**Q: How can I use this to request an adjustment?**
You can use the `generate_accommodation_brief` tool to create a formal request by providing your job tasks, current barriers, and the specific adjustments you need.

**Q: Can I prepare for a meeting with my manager?**
Yes, the `prepare_discussion_agenda` tool helps you create a structured outline for meetings while respecting your defined confidentiality boundaries.

**Q: How do I track the implementation of my request?**
You can use `generate_implementation_plan` to see the logical steps required and `generate_followup_templates` to maintain communication during different phases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-workspace-accommodation-brief](https://vinkius.com/en/ai-agent-connect/accessible-workspace-accommodation-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Workspace Accommodation Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-workspace-accommodation-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Workspace Accommodation Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-workspace-accommodation-brief": {
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
