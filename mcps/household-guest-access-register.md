# Household Guest Access Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-guest-access-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Manage guest entry, verify area permissions, and track departure protocols.

## Description
This MCP server provides a complete management system for residential or facility guest lifecycles. It allows hosts to record guest arrivals, verify if a guest has permission to enter specific zones using `check_guest_access`, monitor currently present visitors with `list_active_guests`, and ensure all exit requirements are met via `validate_departure_tasks`. It acts as a bridge between your AI assistant and the property's access control registry.


## Available Tools (4)
- **check_guest_access**: Verify guest access
- **list_active_guests**: List active guests
- **register_guest_entry**: Record arrival
- **validate_departure_tasks**: Validate departure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Guest Access Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is guest_123 allowed to enter the Kitchen right now?"

**🤖 AI Agent:**
> Yes, guest_123 has permission to enter the Kitchen until 2025-12-31T23:59:59Z.

---

**👤 You:**
> "Who is currently in the house?"

**🤖 AI Agent:**
> There are currently 2 active guests: Alice (Host: John) and Bob (Host: John).

---

**👤 You:**
> "Check if guest_456 has finished their departure tasks: task_01, task_02."

**🤖 AI Agent:**
> All tasks are complete. guest_456 is cleared for departure.


## ❓ FAQ

**Q: How do I check if a guest is allowed in a specific room?**
You can use the `check_guest_access` tool by providing the guest ID, the name of the area, and the current timestamp.

**Q: Can I see everyone currently staying at the property?**
Yes, the `list_active_guests` tool provides a real-time view of all guests currently present.

**Q: How is a guest cleared to leave?**
A guest is cleared once all assigned tasks are finished, which you can verify using `validate_departure_tasks`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-guest-access-register](https://vinkius.com/en/ai-agent-connect/household-guest-access-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Guest Access Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-guest-access-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Guest Access Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-guest-access-register": {
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
