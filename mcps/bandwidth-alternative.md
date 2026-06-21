# Bandwidth MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bandwidth-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage your Bandwidth communications — send SMS and audit calls via AI.

## Description
Empower your AI agent to orchestrate your entire cloud communication infrastructure with **Bandwidth**, the leading platform for enterprise-grade messaging and voice. By connecting Bandwidth to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and retrieve call logs without you ever touching a technical dashboard. Whether you are providing secure alerts or managing global voice infrastructure, your agent acts as a real-time telecom operator, ensuring your communication is always reliable and your usage data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages instantly and retrieve detailed message status and history.
- **Call Auditing** — List all recent voice calls and retrieve real-time call states and metadata.
- **Number Oversight** — List and monitor all phone numbers in service across your account.
- **Application Governance** — List configured Bandwidth applications to ensure your communication logic is correctly applied.
- **Conference Management** — Monitor active conferences and participant data to maintain operational control.

### How it works

1. Subscribe to this server
2. Enter your Bandwidth Account ID, Username, and API Token
3. Start managing your cloud communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication usage and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery statuses and audit call logs without manual dashboard logins.
- **Developers** — perform rapid audits of project configurations and test messaging pipelines through natural language.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_account_info**: Get Bandwidth account details
- **get_call_state**: Get details for a specific call
- **list_applications**: List Bandwidth applications
- **list_calls**: List recent voice calls
- **list_conferences**: List active conferences
- **list_messages**: List recent Bandwidth messages
- **list_phone_numbers**: List phone numbers in service
- **make_call**: Start an outbound voice call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bandwidth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Bandwidth phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' and '+1 987 654 321'. Both are active and ready for voice and SMS services.

---

**👤 You:**
> "Send SMS 'Urgent: system restart required' to +15550123."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your urgent alert to +15550123 using your Bandwidth number. The message ID is xxxxxxxx.

---

**👤 You:**
> "Check for active conferences."

**🤖 AI Agent:**
> I've scanned your account. There is 1 active conference with 3 participants currently connected. Would you like the participant IDs?


## ❓ FAQ

**Q: How do I find my Bandwidth API credentials?**
Log in to your [**Bandwidth Dashboard**](https://dashboard.bandwidth.com/), navigate to **Account** > **API Credentials** to find your Username and Token. Your Account ID is visible in the URL or the Profile section.

**Q: Can the agent check call states?**
Yes. Use the `get_call_state` tool providing the Call ID. Your agent will return real-time status such as 'active', 'completed', or 'busy'.

**Q: Is it possible to manage conferences via the agent?**
Yes. The `list_conferences` tool allows your agent to retrieve all active conferences, helping you monitor multi-party voice sessions in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bandwidth-alternative](https://vinkius.com/mcp/bandwidth-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bandwidth** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bandwidth-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bandwidth** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bandwidth-alternative": {
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
