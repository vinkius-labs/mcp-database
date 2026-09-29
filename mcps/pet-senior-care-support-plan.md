# Pet Senior Care Support Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-senior-care-support-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Non-clinical coordination for senior pet routines and caregiver protocols.

## Description
This MCP connects AI agents to a non-clinical coordination system for senior pet care. It transforms user-provided routines, mobility instructions, and caregiver boundaries into actionable support tools. Use `get_daily_support_arrangement` to generate structured schedules, `get_equipment_readiness_checklist` to verify mobility tools, `get_caregiver_handoff_protocol` for shift transitions, `get_provider_contact_plan` to organize contact hierarchies, and `get_change_escalation_questions` to identify behavioral deviations without medical diagnosis.


## Available Tools (5)
- **get_caregiver_handoff_protocol**: Standardizes the communication between outgoing and incoming caregivers
- **get_change_escalation_questions**: Provides a decision-support tool for identifying deviations without offering medical diagnosis
- **get_daily_support_arrangement**: Generates a structured daily schedule for the caregiver
- **get_equipment_readiness_checklist**: Provides a list of physical tools that must be verified before care begins
- **get_provider_contact_plan**: Organizes the contact hierarchy for the caregiver


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Senior Care Support Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a daily schedule based on this routine: feeding at 8am, walking at 10am, and nap at 1pm. Household is vacant from 9am to 12pm. Caregivers can only perform feeding and walking."

**🤖 AI Agent:**
> The daily support arrangement is ready. The schedule includes feeding at 8:00 AM and walking at 10:00 AM, noting that the household is vacant during the walk. Caregiver boundaries are set to allow only feeding and walking tasks.

---

**👤 You:**
> "I have a harness and a ramp. The harness should be used for all walks, and the ramp is for entering the bed. Create a checklist."

**🤖 AI Agent:**
> The equipment readiness checklist is complete. Items to verify: harness (ensure it is secure for walks) and ramp (ensure it is positioned correctly for bed access).

---

**👤 You:**
> "The pet's normal routine is eating twice a day and walking once. Is there a way to know if something is different?"

**🤖 AI Agent:**
> To identify deviations, you can use the escalation screening questions which focus on observable physical changes, such as whether the pet is moving less than usual.


## ❓ FAQ

**Q: Does this tool provide medical advice?**
No. This system is strictly non-clinical. It uses `get_change_escalation_questions` to identify observable behavioral changes, but it never provides medical diagnoses or clinical guidance.

**Q: How can I ensure my caregiver follows the correct mobility steps?**
You can use `get_equipment_readiness_checklist` to generate a verification list that pairs your chosen equipment with specific mobility instructions.

**Q: How do I manage caregiver shifts?**
Use `get_caregiver_handoff_protocol` to standardize communication between outgoing and incoming caregivers, ensuring continuity of care.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-senior-care-support-plan](https://vinkius.com/en/ai-agent-connect/pet-senior-care-support-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Senior Care Support Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-senior-care-support-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Senior Care Support Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-senior-care-support-plan": {
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
