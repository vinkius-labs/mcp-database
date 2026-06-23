# MightyCall MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mightycall)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Set up a professional virtual phone system with call routing, voicemail, and analytics that makes your small team sound big.

## Description
Connect your **MightyCall** account to any AI agent to streamline your business communications and call center operations. MightyCall provides a powerful REST API (v4) for programmatically managing inbound and outbound calls, retrieving voicemails, and organizing your contact list.

### What you can do

- **Call Orchestration** — List all recent inbound and outbound calls with detailed metadata including status and duration
- **Voicemail Monitoring** — Access and track your voicemails to ensure every customer inquiry is addressed promptly
- **Automated Outreach** — Initiate outgoing calls from your business phone numbers programmatically from your AI agent
- **Contact Management** — Access and manage your business contact list and retrieve detailed profile information
- **Number Intelligence** — List all your business phone numbers to understand your communication infrastructure

### How it works

1. Subscribe to this server
2. Enter your MightyCall Client ID and Client Secret from your dashboard settings
3. Start managing your call center from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support Teams** — monitor call flow and voicemail volume using natural language
- **Sales Professionals** — automate outgoing calls and manage contact records more efficiently
- **Developers** — integrate real-time telephony data and call intelligence into custom business dashboards


## Available Tools (6)
- **create_contact**: Create a new contact
- **list_calls**: List all recent calls
- **list_contacts**: List all contacts
- **list_business_numbers**: List your business phone numbers
- **list_voicemails**: List recent voicemails
- **make_call**: Pass data as a JSON string.

Initiate an outgoing call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MightyCall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent calls in my MightyCall account."

**🤖 AI Agent:**
> I've retrieved your recent calls. You have 5 activities today, including 3 inbound calls from 'Alice Brown' and 2 outbound follow-ups. Would you like to see the duration for any of them?

---

**👤 You:**
> "Show me any unread voicemails."

**🤖 AI Agent:**
> I've checked your voicemails. You have 2 unread messages from yesterday afternoon. One is from an unknown number (+123...) and another from 'Global Tech'.

---

**👤 You:**
> "Make a call from my main number (+198765432) to +123456789."

**🤖 AI Agent:**
> Call initiated successfully! I've triggered the outgoing call from your main number (+198765432) to +123456789. Your desk phone or app should ring shortly.


## ❓ FAQ

**Q: How do I get my MightyCall API credentials?**
Log in to your MightyCall dashboard, navigate to the **API** or **Integrations** section, and generate your Client ID and Client Secret.

**Q: Can I make outgoing calls?**
Yes, use the `make_call` tool and specify which of your business numbers to use as the source and the target destination number.

**Q: Does it track voicemail status?**
Absolutely. The `list_voicemails` tool retrieves your recent messages along with their duration and current status (read/unread).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mightycall](https://vinkius.com/mcp/mightycall)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MightyCall** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mightycall` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MightyCall** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mightycall": {
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
