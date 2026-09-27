# Emergency Repair Contact Roster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-repair-contact-roster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [property-management](../categories/property-management.md)

Generates prioritized emergency response workflows and printable contact rosters.

## Description
This MCP server provides decision-support tools for property managers during emergencies. It uses user-defined contact precedence and after-hours routing rules to generate a prioritized `get_emergency_workflow` call sequence. Users can also use `generate_printable_roster` to create physical contact sheets, `validate_contact_rules` to prevent logical conflicts in routing, and `schedule_roster_audit` to maintain data accuracy.


## Available Tools (4)
- **generate_printable_roster**: Produces a clean, formatted contact sheet for physical use
- **get_emergency_workflow**: Generates a step-by-step prioritized action plan for a specific emergency scenario
- **schedule_roster_audit**: Creates a reminder for the next required maintenance of the contact data
- **validate_contact_rules**: Checks the user's custom precedence and routing rules for logical conflicts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Repair Contact Roster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an emergency workflow for a fire at 123 Maple St at 2024-05-01T02:00:00Z."

**🤖 AI Agent:**
> 1. Call Building Manager (John Doe) at 555-0101. 2. Call Fire Department at 911. 3. Call On-call Electrician at 555-0199. Reminder: Take photos of the fire damage immediately.

---

**👤 You:**
> "Create a printable roster for 456 Oak Ave."

**🤖 AI Agent:**
> Roster for 456 Oak Ave: Building Manager: Jane Smith (555-0202), Insurer: SecureCo (555-0303), Utility: City Water (555-0404).

---

**👤 You:**
> "Schedule a roster audit for 789 Pine Rd every 6 months."

**🤖 AI Agent:**
> The next audit for 789 Pine Rd is scheduled for 2024-11-22.


## ❓ FAQ

**Q: How do I get a prioritized call list for a flood?**
You can use the `get_emergency_workflow` tool by providing the property address, the emergency type (e.g., 'flood'), and the current timestamp.

**Q: Can I check if my contact routing rules are valid?**
Yes, use the `validate_contact_rules` tool to ensure your precedence and routing logic do not contain infinite loops or conflicts.

**Q: How do I create a physical contact sheet?**
Use the `generate_printable_roster` tool with the target property address to produce a formatted contact sheet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-repair-contact-roster](https://vinkius.com/en/ai-agent-connect/emergency-repair-contact-roster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Repair Contact Roster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-repair-contact-roster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Repair Contact Roster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-repair-contact-roster": {
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
