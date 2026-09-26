# Temporary Care Consent Note MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/temporary-care-consent-note)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured, dated handoff documents for temporary childcare.

## Description
This MCP server bridges the gap in authority when a legal guardian temporarily entrusts a child to a caregiver. It synthesizes caregiver information, child routines, and specific decision-making permissions into a formal, dated handoff document. Use `generate_handoff_document` to create the final document, `validate_decision_boundaries` to ensure permissions are safe, `format_routine_summary` to organize schedules, and `build_contact_hierarchy` to prioritize emergency contacts.


## Available Tools (4)
- **build_contact_hierarchy**: Organizes contact information into a prioritized list for emergency use
- **format_routine_summary**: Transforms raw routine descriptions into a readable, organized list
- **generate_handoff_document**: Creates the final formatted document for the caregiver to hold during the care period
- **validate_decision_boundaries**: Ensures the requested permissions do not conflict with safety requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temporary Care Consent Note** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a handoff document for Jane Doe caring for Billy Smith from 2024-06-01 to 2024-06-05. Guardians are John and Mary Smith. Routines: Nap at 1pm, Milk at 8am. Contacts: John (555-0101). Permissions: Medical Triage."

**🤖 AI Agent:**
> Temporary Care Consent Note
Caregiver: Jane Doe
Child: Billy Smith
Guardians: John Smith, Mary Smith
Care Window: 2024-06-01 to 2024-06-05

Permitted Decisions:
- Medical Triage

Daily Routines:
- Nap at 1pm
- Milk at 8am

Emergency Contacts:
- John Smith: 555-0101

Disclaimer: This is a logistical note and not legal advice.

---

**👤 You:**
> "Format these routines for a child: 'Bedtime at 8pm, Breakfast at 7am, Bath time at 6pm'."

**🤖 AI Agent:**
> Morning:
- Breakfast at 7am

Evening:
- Bath time at 6pm
- Bedtime at 8pm

---

**👤 You:**
> "Check if these decisions are valid: ['Medical Triage', 'Nutritional Guidance']."

**🤖 AI Agent:**
> The requested permissions are logically consistent and safe for a temporary caregiver.


## ❓ FAQ

**Q: Is this document legally binding?**
No, this is a logistical handoff tool designed to provide clarity for caregivers. It is not legal advice or a legal contract.

**Q: How do I ensure the caregiver has the right permissions?**
You can use the `validate_decision_boundaries` tool to check if your requested permissions are logically consistent and safe.

**Q: Can I include emergency contact details?**
Yes, the `build_contact_hierarchy` tool helps you organize contact information into a prioritized list for emergency use.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/temporary-care-consent-note](https://vinkius.com/en/ai-agent-connect/temporary-care-consent-note)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Temporary Care Consent Note** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `temporary-care-consent-note` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Temporary Care Consent Note** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "temporary-care-consent-note": {
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
