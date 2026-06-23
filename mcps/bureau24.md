# Bureau24 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bureau24)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Never miss a business call with a live virtual receptionist service that answers, routes, and logs calls professionally.

## Description
Connect your **Bureau24 (bureau24.fr)** virtual secretary account to any AI agent and simplify how you coordinate incoming calls, customer messages, and professional availability through natural conversation.

### What you can do

- **Call Management** — List all calls handled by your virtual receptionist and retrieve detailed notes and participant info.
- **Message Oversight** — List and inspect messages and notifications sent by the Bureau24 service regarding your business activity.
- **Availability Control** — Update your current status (Available, Busy, Away) and provide real-time notes for the secretary on how to handle callers.
- **Contact Directory** — Manage your address book by listing and creating contacts to help the secretary identify regular callers.
- **Instruction Oversight** — Query your standing instructions to verify how calls are being processed by the virtual team.
- **Account Visibility** — Fetch your profile details and verify your current subscription and account metadata.

### How it works

1. Subscribe to this server
2. Enter your Bureau24 API Key (found in your account dashboard)
3. Start managing your virtual secretary from Claude, Cursor, or any MCP client

### Who is this for?

- **Entrepreneurs & Freelancers** — quickly retrieve call notes and update availability status via simple AI commands.
- **Office Managers** — coordinate standing instructions and monitor incoming messages directly from the workspace.
- **Sales Teams** — manage the business directory and verify recent customer calls via the AI assistant.


## Available Tools (10)
- **create_contact**: Add a new contact to your address book
- **get_call**: Get details of a specific call
- **get_me**: fr account and subscription.

Get account information
- **get_message**: Get details of a specific message
- **get_secretary_status**: Get your current secretary status
- **list_calls**: List recent calls received by bureau24.fr
- **list_contacts**: List your address book contacts
- **list_instructions**: List secretary handling instructions
- **list_messages**: List messages from your virtual secretary
- **update_secretary_status**: g., Available, In a Meeting, On Vacation) and provides a note for the secretary.

Update your availability status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bureau24** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent calls handled by my virtual secretary."

**🤖 AI Agent:**
> I've retrieved your call log. You had 3 recent calls: 'John Miller' (Inquiry about pricing), 'Unknown Caller' (Spam), and 'Linda Smith' (Meeting request). Which one would you like to read the full notes for?

---

**👤 You:**
> "Set my status to 'busy' and tell the secretary I am in a workshop until 2 PM."

**🤖 AI Agent:**
> Status updated! I've set your availability to 'busy' in Bureau24 and added the note for the secretary: 'In a workshop until 2 PM'. Callers will be notified accordingly.

---

**👤 You:**
> "Show me the latest message from the Bureau24 service."

**🤖 AI Agent:**
> Fetching messages... Your latest notification (ID: msg_10293) is a summary of today's morning activity: 2 successfully handled calls and 1 urgent callback request from 'Tech Solutions'. Would you like the callback details?


## ❓ FAQ

**Q: Can I update my availability status via AI for the secretary?**
Yes! Use the `update_secretary_status` action. You can provide a new status (like 'busy') and an optional note to tell the secretary exactly what to say to callers.

**Q: How do I see the notes from the last call handled by Bureau24?**
Run the `list_calls` query to find the recent interactions. You can then use `get_call` with the specific Call ID to retrieve all notes and details from the receptionist.

**Q: Is it possible to add a regular customer to my address book via AI?**
Absolutely. Use the `create_contact` tool. Provide the customer's name, phone number, and optional email to help the virtual secretary identify them in future calls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bureau24](https://vinkius.com/mcp/bureau24)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bureau24** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bureau24` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bureau24** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bureau24": {
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
