# Repair Access Arrangement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-access-arrangement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [property-management](../categories/property-management.md)

Coordinates technician visits by validating property access rules and availability.

## Description
This MCP server manages the coordination of onsite repairs. It connects AI agents to property access constraints, technician availability, and preparation requirements. Use `get_access_plan` to generate a confirmed visit schedule and `get_preparation_checklist` to retrieve necessary onsite tasks. It also provides tools like `validate_access_eligibility` and `check_slot_availability` to ensure all visits are authorized and scheduled within permitted hours.


## Available Tools (4)
- **check_slot_availability**: Confirms if there is a technician available within the permitted property access hours
- **get_access_plan**: Generates a finalized schedule and contact plan for a specific repair request
- **get_preparation_checklist**: Provides a list of tasks that must be completed before the technician arrives
- **validate_access_eligibility**: Verifies if a specific contact role is permitted to grant access for a specific item location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Access Arrangement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you schedule a repair for repair-123 on 2025-05-10?"

**🤖 AI Agent:**
> Your repair visit is confirmed for 2025-05-10 between 10:00 AM and 12:00 PM. The authorized contact is the Building Manager.

---

**👤 You:**
> "What do I need to prepare for repair-456?"

**🤖 AI Agent:**
> Please clear the path to the water meter and ensure the rear gate is unlocked before the technician arrives.

---

**👤 You:**
> "Is there any technician availability at location-789 on 2025-06-01?"

**🤖 AI Agent:**
> Yes, there are two available slots between 09:00 AM and 11:00 AM for that location.


## ❓ FAQ

**Q: How do I schedule a repair visit?**
You can use the `get_access_plan` tool by providing the unique repair ID and your requested date to receive a confirmed schedule.

**Q: What should I do before the technician arrives?**
Use the `get_preparation_checklist` tool with your repair ID to see the specific tasks required for your location.

**Q: Can I check if a specific person is allowed to grant access?**
Yes, the `validate_access_eligibility` tool allows you to verify if a contact role is permitted to authorize access for a specific location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-access-arrangement](https://vinkius.com/en/ai-agent-connect/repair-access-arrangement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Access Arrangement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-access-arrangement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Access Arrangement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-access-arrangement": {
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
