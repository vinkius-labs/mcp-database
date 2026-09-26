# Apartment Emergency Coordination Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/apartment-emergency-coordination-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Synthesize building rules and household profiles into actionable emergency preparedness documentation.

## Description
This MCP server connects AI agents to emergency preparedness workflows. It processes building management constraints, unit logistics, and household profiles to generate critical safety documents. Use `generate_resident_contact_card` to create responder summaries, `create_management_notification_plan` to align with building protocols, `map_supply_placement_tasks` to organize emergency kits near exits, and `schedule_annual_review` to maintain plan validity.


## Available Tools (4)
- **create_management_notification_plan**: Determines how and when to alert building management
- **generate_resident_contact_card**: Creates a high-level summary of the household identity and emergency contact details
- **map_supply_placement_tasks**: Generates a checklist of where to store emergency supplies
- **schedule_annual_review**: Determines the next required audit date for the coordination plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apartment Emergency Coordination Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a contact card for a household with two adults and one child with asthma."

**🤖 AI Agent:**
> Resident Contact Card: Adults: John Doe, Jane Doe; Child: Billy Doe (Asthma). Emergency Contacts: John Doe (555-0101), Jane Doe (555-0102).

---

**👤 You:**
> "Create a notification plan for a Gas Leak in Unit 4B."

**🤖 AI Agent:**
> Notification Plan: Primary Contact: Building Management; Method: Emergency Phone Call; Priority: High; Required Action: Evacuate unit immediately and contact building maintenance.

---

**👤 You:**
> "Where should I store my emergency supplies given my unit has a main exit in the hallway?"

**🤖 AI Agent:**
> Recommended Location: Place emergency kits in the central hallway area adjacent to the designated main exit.


## ❓ FAQ

**Q: How does this tool handle conflicting exit routes?**
Management-issued safety protocols and exit routes take absolute precedence over individual resident preferences.

**Q: Can I include pets in the emergency planning?**
Yes, the `map_supply_placement_tasks` tool specifically includes tasks for pet-specific supplies if pets are listed in the household members.

**Q: How often should the emergency plan be updated?**
Plans require a yearly re-validation. You can use `schedule_annual_review` to determine the next required audit date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/apartment-emergency-coordination-plan](https://vinkius.com/en/ai-agent-connect/apartment-emergency-coordination-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apartment Emergency Coordination Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apartment-emergency-coordination-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apartment Emergency Coordination Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apartment-emergency-coordination-plan": {
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
