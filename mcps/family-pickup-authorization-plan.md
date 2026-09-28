# Family Pickup Authorization Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-pickup-authorization-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Manage and verify child pickup authorizations against institutional security rules.

## Description
This MCP server provides a secure management system for coordinating child pickups. It allows AI agents to verify authorized individuals against specific institutional requirements, such as ID types and pickup windows. Use `list_authorization_matrix` to view permissions, `get_emergency_contacts` for urgent situations, and `validate_pickup_attempt` to confirm real-time authorization for a specific person and child.


## Available Tools (4)
- **get_emergency_contacts**: Retrieves a high-priority list of individuals permitted to pick up children in urgent or unplanned situations
- **generate_update_tasks**: Identifies necessary administrative actions to keep the authorization plan valid and current
- **list_authorization_matrix**: Provides a complete overview of who is authorized to pick up which children according to institutional rules
- **validate_pickup_attempt**: Confirms if a specific person is cleared to pick up a specific child at a specific time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Pickup Authorization Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the authorization matrix for institution ID 'school-123'."

**🤖 AI Agent:**
> The authorization matrix for school-123 shows that Alice Smith is cleared with a driver's license, and Bob Jones is not cleared due to an expired ID.

---

**👤 You:**
> "Who are the emergency contacts for Charlie?"

**🤖 AI Agent:**
> The emergency contacts for Charlie are Sarah Miller (Mother, 555-0123) and David Wilson (Uncle, 555-0456).

---

**👤 You:**
> "Is Jane Doe authorized to pick up Timmy at 'daycare-45' using a passport?"

**🤖 AI Agent:**
> Yes, Jane Doe is authorized to pick up Timmy at daycare-45 using a passport.


## ❓ FAQ

**Q: How can I see who is allowed to pick up my child?**
You can use the `list_authorization_matrix` tool by providing the specific institution ID to see a complete overview of authorized persons.

**Q: What happens if an authorization has expired?**
Expired authorizations will be identified by the `generate_update_tasks` tool, which helps you manage administrative renewals.

**Q: Can I verify a pickup in real-time?**
Yes, the `validate_pickup_attempt` tool confirms if a person is cleared to pick up a child based on their ID and the institution's rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-pickup-authorization-plan](https://vinkius.com/en/ai-agent-connect/family-pickup-authorization-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Pickup Authorization Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-pickup-authorization-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Pickup Authorization Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-pickup-authorization-plan": {
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
