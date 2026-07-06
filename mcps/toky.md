# Toky MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/toky)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Handle business calls from anywhere with a cloud phone system that includes IVR, call recording, and CRM integration.

## Description
Connect your **Toky** cloud phone system account to any AI agent and simplify how you manage your business communications, call logs, and SMS outreach through natural conversation.

### What you can do

- **Call Management** — List and search call history, retrieve detailed metadata, and monitor recent voicemails.
- **SMS Automation** — Send individual text messages to customers and leads directly via AI commands.
- **Contact Oversight** — List, create, and manage your phone directory to keep customer data synchronized.
- **Team Coordination** — Query agent lists and retrieve detailed profiles for your communication team.
- **Operational Status** — Fetch detailed metadata for specific calls or voicemails to understand interaction context.
- **Communication Visibility** — Monitor your cloud telephony activities directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Toky API Key (found in your developer settings)
3. Start managing your cloud phone system from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & Support Teams** — quickly send SMS follow-ups and retrieve call logs via simple AI commands.
- **Operations Managers** — monitor agent availability and verify communication history across the team.
- **Business Owners** — maintain an organized record of customer interactions and voicemails directly from the workspace.


## Available Tools (10)
- **get_call**: Get details for a specific Toky call
- **get_contact**: Get details for a specific Toky contact
- **get_voicemail**: Get details for a specific Toky voicemail
- **list_agents**: Use limit and offset for pagination.

List Toky agents
- **list_calls**: Use limit and offset for pagination.

List Toky calls
- **list_contacts**: Use limit and offset for pagination.

List Toky contacts
- **list_voicemails**: Use limit and offset for pagination.

List Toky voicemails
- **send_sms**: Send an SMS via Toky
- **create_contact**: Create a new Toky contact
- **get_agent**: Get details for a specific Toky agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Toky** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active agents in my Toky account."

**🤖 AI Agent:**
> I've retrieved your agents. You have 3 active users: 'Alex Rivera' (Available), 'Sarah Smith' (On a call), and 'Mike Ross'. Which one would you like more details on?

---

**👤 You:**
> "Show me the last 3 calls from today."

**🤖 AI Agent:**
> I've fetched the call history. Today you had: 1 Incoming from +15550199 (Missed), 1 Outgoing to John Doe (Success, 5m), and 1 Incoming from Unknown (Success, 2m). Shall I retrieve the recording for the John Doe call?

---

**👤 You:**
> "Send an SMS to 5511999999999 saying 'Your consultation is confirmed for tomorrow'."

**🤖 AI Agent:**
> SMS message sent! I've transmitted your confirmation text to 5511999999999. The transmission ID is SMS-88231. Your customer should receive it shortly.


## ❓ FAQ

**Q: Can I see my recent call history via AI?**
Yes! Use the `list_calls` tool. Your agent will retrieve the history of all incoming and outgoing calls, including durations and participant details.

**Q: How do I send an SMS to a customer using the AI?**
Use the `send_sms` action. Provide the destination phone number and your message text. The agent will trigger the SMS transmission through your Toky account instantly.

**Q: Is it possible to check for new voicemails via AI?**
Absolutely. Run the `list_voicemails` query. The agent will retrieve a list of all recorded voicemails, which you can then inspect for specific interaction details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/toky](https://vinkius.com/mcp/toky)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Toky** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `toky` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Toky** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "toky": {
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
