# Family Event Consent Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-event-consent-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [management](../categories/management.md)

Manage attendee permissions, restrictions, and consent status for family events.

## Description
This MCP server provides tools to manage attendee safety and compliance for family-oriented gatherings. Use `get_attendee_profile` to view individual details, `validate_consent_for_event` to check authorization, `filter_by_restriction` to identify specific needs like allergies, and `generate_staff_roster` to produce a complete, staff-ready table for event execution.


## Available Tools (4)
- **filter_by_restriction**: Find all attendees who share a specific restriction
- **generate_staff_roster**: Produce the final, staff-ready table containing all necessary information for event execution
- **get_attendee_profile**: Retrieve the complete individual profile for a specific attendee
- **validate_consent_for_event**: Check if an attendee has provided sufficient acknowledgment for a specific event date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Event Consent Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is John Doe authorized to participate in the event on 2024-07-04?"

**🤖 AI Agent:**
> Yes, John Doe is authorized to participate in the event on 2024-07-04.

---

**👤 You:**
> "Show me the profile for attendee ID 123."

**🤖 AI Agent:**
> Attendee 123 is Jane Smith, age 34. Her contact info is jane.smith@email.com. She has permission for photography and no active restrictions.

---

**👤 You:**
> "Generate a roster for the event on 2024-12-25 including permissions."

**🤖 AI Agent:**
> The roster for 2024-12-25 includes: Alice (Authorized, No restrictions, 555-0101, Photography), Bob (Authorized, Nut Allergy, 555-0102, No permissions).


## ❓ FAQ

**Q: How can I check if an attendee is cleared for an event?**
You can use the `validate_consent_for_event` tool to verify if an attendee has provided sufficient acknowledgment for a specific date.

**Q: Can I find all attendees with specific medical restrictions?**
Yes, the `filter_by_restriction` tool allows you to find all attendees who share a specific restriction, such as a dietary requirement.

**Q: How do I get a list of everyone attending on a specific day?**
Use the `generate_staff_roster` tool to produce a finalized, staff-ready table for any given event date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-event-consent-register](https://vinkius.com/en/ai-agent-connect/family-event-consent-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Event Consent Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-event-consent-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Event Consent Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-event-consent-register": {
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
