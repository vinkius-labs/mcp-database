# Outage Readiness & Coordination Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outage-readiness-coordination-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms household data into actionable outage checklists, communication protocols, and supply requirements.

## Description
This MCP server acts as a bridge between your household data and emergency preparedness. It processes dependencies, backup options, and contact information to generate prioritized pre-outage checklists using `get_pre_outage_checklist`, structured communication plans via `generate_communication_plan`, and specific supply actions through `calculate_supply_actions`. It also provides a recovery directory using `get_recovery_contact_list` to ensure safe restoration of services after an event.


## Available Tools (4)
- **calculate_supply_actions**: Determines the necessary physical supplies and specific actions needed based on household requirements
- **generate_communication_plan**: Establishes how the household will stay informed and how members will contact one another
- **get_pre_outage_checklist**: Generates a prioritized list of tasks to complete before a predicted outage occurs
- **get_recovery_contact_list**: Provides a structured directory for restoring services and verifying safety after the outage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outage Readiness & Coordination Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a pre-outage checklist for a household with an elderly person needing mobility support and a pet."

**🤖 AI Agent:**
> Priority: High. Tasks: 1. Ensure mobility aids are fully charged. 2. Stock up on specialized pet food. 3. Verify flashlight and battery availability for accessibility.

---

**👤 You:**
> "Create a communication plan using my contact list and the local utility's instructions."

**🤖 AI Agent:**
> Primary Channel: SMS. Contact Hierarchy: 1. Household Members, 2. Trusted Contacts, 3. Local Utility Provider.

---

**👤 You:**
> "What supplies do I need if I have a portable generator?"

**🤖 AI Agent:**
> Items to acquire: Fuel for generator, extension cords. Storage: Keep fuel in approved containers away from living areas.


## ❓ FAQ

**Q: How do I generate a checklist before an outage?**
You can use the `get_pre_outage_checklist` tool by providing your household dependencies, available backup options, and any accessibility needs.

**Q: Can this tool help with communication during an emergency?**
Yes, the `generate_communication_plan` tool establishes a contact hierarchy and primary communication channels based on your local provider guidance.

**Q: How are supply needs calculated?**
The `calculate_supply_actions` tool determines necessary items and storage instructions by analyzing your household dependencies and backup resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outage-readiness-coordination-plan](https://vinkius.com/en/ai-agent-connect/outage-readiness-coordination-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outage Readiness & Coordination Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outage-readiness-coordination-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outage Readiness & Coordination Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outage-readiness-coordination-plan": {
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
