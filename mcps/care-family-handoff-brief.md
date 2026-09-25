# Care Family Handoff Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-family-handoff-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform raw caregiving data into structured, role-based handoff briefs for seamless transitions.

## Description
Ensure continuity of care with professional handoff documentation. This MCP server provides tools to transform raw caregiver information--routines, tasks, appointments, and privacy rules--into structured briefs tailored to specific recipients. Use `generate_handoff_brief` to create role-based documents for professional caregivers or family members, `identify_priority_actions` to pinpoint critical first-48-hour tasks, `flag_information_gaps` to prevent care errors by identifying missing data, and `create_acknowledgment_checklist` to ensure safety and compliance with spending and privacy constraints.


## Available Tools (4)
- **create_acknowledgment_checklist**: Generate a list of items the receiver must confirm they have understood and accepted
- **flag_information_gaps**: Identify missing or ambiguous information that could lead to care errors
- **generate_handoff_brief**: Transform raw input data into a structured, professional handoff document tailored to a specific recipient role
- **identify_priority_actions**: Extract the most urgent items that require attention within the first 48 hours of the handoff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Family Handoff Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a handoff brief for a Professional Caregiver based on these routines and tasks."

**🤖 AI Agent:**
> Handoff Brief: Professional Caregiver

Status: Active Transition

Approved Tasks:
- Medication administration
- Mobility assistance

Immediate Priorities:
- 10:00 AM Medication check

Access Details:
- Keypad code: 1234

---

**👤 You:**
> "What are the most urgent tasks for the next 48 hours?"

**🤖 AI Agent:**
> The immediate priorities for the next 48 hours are: 1. Attend the doctor's appointment on Tuesday at 2 PM, and 2. Complete the scheduled physical therapy session on Wednesday morning.

---

**👤 You:**
> "Are there any missing pieces of information in my care plan?"

**🤖 AI Agent:**
> Yes, the contact list is missing a primary emergency contact, and the spending limit for groceries does not specify an authorization method.


## ❓ FAQ

**Q: How does the tool handle different recipient roles?**
The `generate_handoff_brief` tool uses role-based templates to filter information. For example, a Professional Caregiver receives technical and operational details, while a Family Member receives a warmer summary focused on routines and emotional well-being.

**Q: Can I identify urgent tasks for a new caregiver?**
Yes, you can use the `identify_priority_actions` tool to extract the most critical tasks and appointments that must be addressed within the first 48 hours of a transition.

**Q: How does this ensure care safety?**
Safety is maintained through `flag_information_gaps` to catch missing details and `create_acknowledgment_checklist` to confirm the receiver understands privacy rules and spending limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-family-handoff-brief](https://vinkius.com/en/ai-agent-connect/care-family-handoff-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Family Handoff Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-family-handoff-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Family Handoff Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-family-handoff-brief": {
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
