# Temporary Guardian Information Pack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/temporary-guardian-information-pack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [documentation](../categories/documentation.md)

Compile comprehensive, printable handoff documentation for temporary caregivers.

## Description
This MCP server provides a suite of tools to assemble a complete, printable handoff packet for temporary caregivers. It bridges the gap between child safety data and caregiver readiness by aggregating child profiles, daily routines, medical records, and emergency contacts into a single, organized document. Use `generate_handoff_packet` to create the final summary, or use individual tools like `fetch_child_profile`, `query_routines`, `get_emergency_contacts`, and `verify_permissions` to retrieve specific safety and scheduling details.


## Available Tools (5)
- **fetch_child_profile**: Retrieves the core identity and safety information for a specific child
- **generate_handoff_packet**: Creates a complete, printable summary of all necessary information for a temporary guardian
- **get_emergency_contacts**: Retrieves the structured contact list for the child
- **query_routines**: Retrieves the daily schedules and behavioral patterns for a child
- **verify_permissions**: Checks what specific authorities the temporary guardian has been granted


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Temporary Guardian Information Pack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a full handoff packet for child ID 'child_123' and guardian ID 'guard_456' including medical and routine details."

**🤖 AI Agent:**
> Child Profile: Alex Smith (DOB: 2018-05-12). Allergies: Peanuts. Routines: Nap at 1:00 PM. Emergency Contact: Jane Doe (Mother) - 555-0123. Medical: Authorized for basic first aid.

---

**👤 You:**
> "What are the daily routines for child 'child_789'?"

**🤖 AI Agent:**
> The daily routine for child 'child_789' includes meal times at 8:00 AM, 12:00 PM, and 6:00 PM, with a sleep schedule starting at 8:30 PM.

---

**👤 You:**
> "Check the permissions for guardian 'guard_999' regarding child 'child_123'."

**🤖 AI Agent:**
> Guardian 'guard_999' has medical consent and dietary authority, but does not have travel authorization for child 'child_123'.


## ❓ FAQ

**Q: How do I create the final printable document?**
You can use the `generate_handoff_packet` tool, which aggregates all necessary child and guardian information into a single formatted text block.

**Q: Can I include medical details in the packet?**
Yes, by setting the `includeMedicalDetails` parameter to true when calling `generate_handoff_packet`, the tool will merge medical records with current permissions.

**Q: How are emergency contacts organized?**
Contacts are retrieved via `get_emergency_contacts` and are automatically sorted by their priority level, from primary to emergency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/temporary-guardian-information-pack](https://vinkius.com/en/ai-agent-connect/temporary-guardian-information-pack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Temporary Guardian Information Pack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `temporary-guardian-information-pack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Temporary Guardian Information Pack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "temporary-guardian-information-pack": {
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
