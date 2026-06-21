# Plivo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plivo-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your Plivo communications — send SMS and audit calls via AI.

## Description
Empower your AI agent to orchestrate your entire cloud communication infrastructure with **Plivo**, the enterprise-grade platform for messaging and voice. By connecting Plivo to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and retrieve call logs without you ever touching a technical console. Whether you are providing customer notifications or managing corporate voice lines, your agent acts as a real-time telecom operator, ensuring your communication is always reliable and your usage data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages instantly and retrieve detailed message status and history.
- **Call Auditing** — List all recent voice calls and retrieve metadata for each, including duration and status.
- **Number Oversight** — List and monitor all phone numbers associated with your account.
- **Pricing Insights** — Retrieve detailed pricing information for messaging and voice services across different countries.
- **Application Governance** — List configured Plivo applications to ensure your communication logic is correctly applied.

### How it works

1. Subscribe to this server
2. Enter your Plivo Auth ID and Auth Token
3. Start managing your cloud communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication usage and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery statuses and audit call logs without manual dashboard logins.
- **Developers** — perform rapid audits of project configurations and test messaging pipelines through natural language.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_account**: Get Plivo account details
- **get_call**: Get details for a specific call
- **get_message**: Get details for a specific message
- **list_applications**: List Plivo applications
- **list_calls**: List recent voice calls
- **list_messages**: List recent SMS messages
- **list_phone_numbers**: List Plivo phone numbers
- **list_pricing**: Get pricing for a country
- **make_call**: Start an outbound call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Plivo phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' and '+44 987 654 321'. Both are active and configured for voice and SMS.

---

**👤 You:**
> "Send SMS 'Your appointment is confirmed' to +15550123."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your confirmation to +15550123 using your Plivo number. The message UUID is xxxxxxxx.

---

**👤 You:**
> "What is the SMS pricing for Brazil?"

**🤖 AI Agent:**
> I've retrieved the pricing for Brazil (BR). Outbound SMS is $0.05 per message, and inbound is free for mobile numbers. Would you like the voice rates as well?


## ❓ FAQ

**Q: How do I find my Plivo Auth ID and Auth Token?**
Log in to your [**Plivo Dashboard**](https://console.plivo.com/dashboard/), and you will find your Auth ID and Auth Token right on the front page. Copy and paste them below.

**Q: Can the agent check international pricing?**
Yes. Use the `list_pricing` tool providing the country ISO code (e.g., 'US', 'GB', 'BR'). Your agent will return detailed rates for inbound and outbound messages and calls.

**Q: Is it possible to trigger an outbound call via the agent?**
Yes. The `make_call` tool allows your agent to start an outbound voice call. You must provide a valid `answerUrl` which Plivo will fetch for instructions when the call is answered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plivo-alternative](https://vinkius.com/mcp/plivo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plivo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plivo-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plivo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plivo-alternative": {
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
