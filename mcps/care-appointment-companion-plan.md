# Care Appointment Companion Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-appointment-companion-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Logistical coordination for non-medical companions attending healthcare appointments.

## Description
This MCP server manages the logistical coordination between caregivers and non-medical companions. It ensures companions are prepared with clear itineraries, access checklists, and defined note-sharing permissions. Use `generate_companion_itinerary` to calculate travel buffers, `create_access_checklist` for facility entry requirements, `setup_note_sharing_permissions` to respect family consent, and `generate_followup_tasks` to manage post-appointment actions.


## Available Tools (4)
- **generate_companion_itinerary**: Creates a complete timeline of the appointment day including travel and arrival buffers
- **generate_followup_tasks**: Produces a list of actions for the companion to take after the appointment is over
- **setup_note_sharing_permissions**: Defines the boundaries of what the companion can record and share based on family preferences
- **create_access_checklist**: Generates a list of items and verifications needed for the companion to enter and navigate the facility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Appointment Companion Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an itinerary for an appointment at 2:00 PM. Travel takes 30 minutes and I want a 15-minute arrival buffer."

**🤖 AI Agent:**
> Your departure time is 1:15 PM. You will arrive at the facility at 1:45 PM, providing a 15-minute buffer before your 2:00 PM appointment.

---

**👤 You:**
> "What do I need to bring for a hospital visit where ID is required?"

**🤖 AI Agent:**
> You should bring your valid photo identification and follow the facility's check-in procedures.

---

**👤 You:**
> "Set permissions for 'Logistics Only' consent and allow non-medical observations."

**🤖 AI Agent:**
> Permissions set: Recording is strictly limited to time and movement. Non-medical observations like mood or mobility are permitted.


## ❓ FAQ

**Q: Can the companion provide medical advice?**
No. The companion is a non-medical facilitator. They must never provide medical diagnoses or suggest treatments.

**Q: How are travel buffers handled?**
The `generate_companion_itinerary` tool automatically calculates arrival and transit buffers to ensure a smooth schedule.

**Q: How is patient privacy protected?**
Privacy is managed via `setup_note_sharing_permissions`, which enforces the family's specific consent levels for documentation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-appointment-companion-plan](https://vinkius.com/en/ai-agent-connect/care-appointment-companion-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Appointment Companion Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-appointment-companion-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Appointment Companion Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-appointment-companion-plan": {
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
