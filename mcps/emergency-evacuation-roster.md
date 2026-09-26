# Emergency Evacuation Roster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-evacuation-roster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Generate prioritized evacuation checklists and verify mobility readiness for household members and pets.

## Description
This MCP server provides critical tools for managing household evacuations. It allows AI agents to synthesize prioritized action checklists using `generate_evacuation_checklist`, verify if transport plans meet the physical needs of all members with `verify_mobility_readiness`, identify specific safe zones via `resolve_meeting_point`, and manage animal safety with `list_pet_evacuation_tasks`. It ensures every person and pet is accounted for in emergency scenarios.


## Available Tools (4)
- **list_pet_evacuation_tasks**: Generates a specialized sub-checklist specifically for the care and transport of animals
- **resolve_meeting_point**: Determines the specific destination for a person based on their assigned zone
- **verify_mobility_readiness**: Evaluates if the current transport and meeting point plan satisfies the physical requirements of all members
- **generate_evacuation_checklist**: Synthesizes a prioritized, step-by-step action list for a specific household configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Evacuation Roster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an evacuation checklist for a family of three with one dog."

**🤖 AI Agent:**
> 1. Contact primary contact. 2. Secure leash for Buddy. 3. Move dependent member to Neighborhood meeting point via car. 4. Move mobile members to Immediate meeting point.

---

**👤 You:**
> "Is the current transport plan safe for a member in a wheelchair?"

**🤖 AI Agent:**
> No, the current plan is unsafe because the assigned bicycle transport is not compatible with the wheelchair mobility status of the member.

---

**👤 You:**
> "Where should the primary contact go during an evacuation?"

**🤖 AI Agent:**
> The primary contact should proceed to the Regional meeting point, which is a 5-mile drive away and offers a high safety level.


## ❓ FAQ

**Q: How do I generate a full evacuation plan?**
You can use the `generate_evacuation_checklist` tool by providing household members, meeting points, transport assignments, pet requirements, and the contact order.

**Q: Can this tool check if my transport plan is safe for everyone?**
Yes, the `verify_mobility_readiness` tool evaluates if assigned transport methods are compatible with the mobility status of all household members.

**Q: How are pets handled in the evacuation process?**
The `list_pet_evacuation_tasks` tool generates specific tasks for animals, such as securing leashes or preparing carriers, to ensure they are ready for transport.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-evacuation-roster](https://vinkius.com/en/ai-agent-connect/emergency-evacuation-roster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Evacuation Roster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-evacuation-roster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Evacuation Roster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-evacuation-roster": {
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
