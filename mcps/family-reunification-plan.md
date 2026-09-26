# Family Reunification Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-reunification-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [preparedness](../categories/preparedness.md)

Generate structured emergency reunification assets, contact hierarchies, and drill schedules.

## Description
This MCP server provides essential tools for household emergency preparedness. It allows AI agents to generate printable reunification cards, build resilient contact trees, assign critical emergency roles, and create structured drill schedules. Use `generate_reunification_card` to create immediate access to meeting points and authorized pickups, `build_contact_tree` to organize communication flows, `assign_emergency_roles` to define responsibilities, and `create_drill_schedule` to plan regular practice scenarios.


## Available Tools (4)
- **create_drill_schedule**: Generates a structured plan for practicing reunification procedures
- **generate_reunification_card**: Creates a concise, printable summary of essential reunification data
- **assign_emergency_roles**: Maps family members to critical emergency roles
- **build_contact_tree**: Organizes household contacts into a logical hierarchy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Reunification Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a reunification card for my family with our home at 123 Maple St, school at West Elementary, and work at Downtown Corp. Our meeting points are the local park, the community center, and the library in the next city."

**🤖 AI Agent:**
> Your reunification card is ready. Primary Location: Local Park (123 Maple St area). Secondary Location: Community Center. Tertiary Location: City Library. Authorized Pickups: Mom, Dad.

---

**👤 You:**
> "Help me assign emergency roles for my family members: Alice, Bob, and Charlie. I need a Communication Lead and a Logistics Coordinator."

**🤖 AI Agent:**
> Roles assigned: Alice is the Communication Lead, and Bob is the Logistics Coordinator. Charlie remains unassigned.

---

**👤 You:**
> "Build a contact tree for my household. Contacts are: Alice (ID: 1, Role: Lead, Backup: Bob), Bob (ID: 2, Role: Support, Backup: Alice), and the coordinator is Alice."

**🤖 AI Agent:**
> Contact tree successfully built with Alice as the root coordinator and Bob as the primary backup.


## ❓ FAQ

**Q: What is a reunification card?**
A reunification card is a concise, printable summary of essential data like meeting locations and authorized contacts, created using `generate_reunification_card`.

**Q: How do I ensure my communication chain works?**
You can use `build_contact_tree` to organize your household contacts into a logical hierarchy with designated backups to prevent communication gaps.

**Q: Can I schedule regular practice drills?**
Yes, the `create_drill_schedule` tool generates a structured plan for practicing reunification procedures based on your preferred frequency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-reunification-plan](https://vinkius.com/en/ai-agent-connect/family-reunification-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Reunification Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-reunification-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Reunification Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-reunification-plan": {
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
