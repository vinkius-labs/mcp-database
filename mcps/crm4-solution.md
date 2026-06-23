# crm4 solution MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crm4-solution)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Italian lead management and call center CRM.

## Description
The crm4 solution MCP server enables your AI agent to manage leads, campaigns, and call center activities. Automate your customer outreach via SMS, WhatsApp, and phone calls directly from your chat.


## Available Tools (12)
- **add_contact_to_list**: Add a contact to a specific distribution list
- **create_contact**: Create a new contact in the CRM
- **delete_contact**: Permanently remove a contact
- **get_contact**: Retrieve details for a specific contact
- **list_calls**: Retrieve call center activity logs
- **list_campaigns**: List all marketing/calling campaigns
- **list_contacts**: List all contacts/leads
- **list_contact_lists**: List all contact distribution lists
- **search_contacts**: Search for contacts using filters
- **send_sms**: Send an SMS message to a contact
- **send_whatsapp**: Send a WhatsApp message (requires approved template)
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **crm4 solution** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in CRM4."

**🤖 AI Agent:**
> I found 3 active campaigns. The most engaged one is 'Summer Promo' with a 45% contact rate.

---

**👤 You:**
> "Send a 'Welcome' WhatsApp message to '+123456789'."

**🤖 AI Agent:**
> The WhatsApp template 'Welcome' has been queued for delivery to +123456789.

---

**👤 You:**
> "Add John Doe as a new lead in the system."

**🤖 AI Agent:**
> Lead 'John Doe' successfully created and added to the unassigned queue.


## ❓ FAQ

**Q: Does it support WhatsApp templates?**
Yes, but they must be approved in your CRM4 dashboard before sending via API.

**Q: Can I automate outbound call campaigns?**
Yes, you can manage and query the status of your call center campaigns directly via the agent.

**Q: Is lead management completely available via chat?**
Yes, the AI can query, create, and update lead records continuously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crm4-solution](https://vinkius.com/mcp/crm4-solution)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **crm4 solution** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crm4-solution` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **crm4 solution** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crm4-solution": {
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
