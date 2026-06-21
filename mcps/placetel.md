# Placetel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/placetel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage Placetel users, devices, numbers, and calls.

## Description
# Placetel

The Placetel MCP Server allows AI agents to interact with your Placetel PBX data seamlessly.

### What you can do
- Retrieve users, SIP users, and groups.
- Access phone numbers and routing plans.
- Manage devices and call detail records (CDRs).

### How it works
Connect your Placetel account via your API Token to manage your VoIP configurations dynamically.


## Available Tools
- **get_group**: Get details for a specific group
- **get_sip_user**: Get details for a specific SIP user
- **get_user**: Get details for a specific user
- **list_call_detail_records**: List Call Detail Records (CDRs)
- **list_calls**: List active or recent calls
- **list_devices**: List all devices
- **list_groups**: List all Placetel groups
- **list_numbers**: List all Placetel numbers
- **list_sip_users**: List all Placetel SIP users
- **list_users**: List all Placetel users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Placetel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all devices in Placetel."

**🤖 AI Agent:**
> I retrieved your devices. Here are the active ones: 'Desk Phone 1', 'Softphone - John'.

---

**👤 You:**
> "Get call details from today."

**🤖 AI Agent:**
> Here are your Call Detail Records for today, including 5 inbound calls and 3 outbound calls.

---

**👤 You:**
> "List all users in my account."

**🤖 AI Agent:**
> You have 2 users in your account: 'Admin' and 'Sales'.


## ❓ FAQ

**Q: Where do I find my API Token?**
Your API Token can be found in your Placetel web portal under Integrations > Web API.

**Q: What access does this MCP need?**
It requires the REST API Token, giving access to users, calls, numbers, and devices.

**Q: Can I initiate phone calls using this server?**
Currently, this integration supports retrieving Placetel data like CDRs and configurations. Call initiation via CTI will be added in a future update.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/placetel](https://vinkius.com/mcp/placetel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Placetel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `placetel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Placetel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "placetel": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
