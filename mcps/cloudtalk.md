# CloudTalk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudtalk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Modern cloud-based phone system designed for sales and support teams, offering seamless call center automation.

## Description
CloudTalk is a modern cloud-based phone system designed for sales and support teams, offering seamless call center automation and CRM integrations. It empowers agents to handle calls efficiently across the globe. You can easily fetch call logs, search contacts, and retrieve analytics metrics programmatically.


## Available Tools (8)
- **create_contact**: Provide at least a name or email.

Create a new contact in CloudTalk
- **delete_contact**: Deletes the contact and all associated data.

Permanently remove a contact from CloudTalk
- **get_contact**: Retrieve detailed information about a specific contact
- **list_agents**: Retrieve a list of agents from CloudTalk
- **list_calls**: Supports filtering by agent and direction.

Retrieve a list of calls from CloudTalk
- **list_contacts**: Supports pagination and filtering by email or phone number.

Retrieve a list of contacts from CloudTalk
- **make_call**: Provide the from/to numbers.

Initiate a phone call between an agent and a destination number
- **update_contact**: Provide the contactId and any fields to update.

Update an existing contact in CloudTalk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudTalk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 calls in CloudTalk."

**🤖 AI Agent:**
> Here are the last 10 calls:
1. +1-555-0123 → Sales Team (4m 32s, completed)
2. +44-20-7946 → Support (2m 15s, completed)
3. +1-555-0456 → Marketing (missed)
... Showing 3 of 10. Total talk time: 28 minutes.

---

**👤 You:**
> "Find the contact with email 'john.doe@example.com' in CloudTalk."

**🤖 AI Agent:**
> Found contact: John Doe (john.doe@example.com). Phone: +1-555-0199. Company: Acme Corp. Agent: Sarah M. Last call: March 15, 2025 (3m 45s). Total interactions: 12.

---

**👤 You:**
> "Initiate a call to +123456789 from my CloudTalk extension."

**🤖 AI Agent:**
> Call initiated to +123456789 from your extension (ext. 204). Status: ringing. Call ID: call_8f3a2b. You'll receive a notification when the call connects.


## ❓ FAQ

**Q: How do I find my CloudTalk API credentials?**
You can find your API Access Key ID and Secret in the CloudTalk Dashboard under Account > Settings > API keys.

**Q: Can I record calls with this MCP server?**
While the server doesn't initiate recording itself, it can retrieve links to call recordings if they were enabled in your CloudTalk settings.

**Q: Which numbers can I use for making calls?**
You can use any of your verified CloudTalk numbers as the sender and any valid international phone number as the recipient.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudtalk](https://vinkius.com/mcp/cloudtalk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudTalk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudtalk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudTalk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudtalk": {
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
