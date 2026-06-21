# Mainstay (AdmitHub) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mainstay-admithub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-engagement](../categories/customer-engagement.md)

Student engagement and behavioral intelligence — manage contacts, campaigns, and AI nudges via AI.

## Description
Connect your **Mainstay (formerly AdmitHub)** account to your AI agent to unlock research-backed student engagement and behavioral intelligence. From managing large-scale student contact lists to monitoring AI-powered nudges and auditing campaign performance, your agent handles student success workflows through natural conversation.

### What you can do

- **Contact Management** — List, retrieve, and update student records to ensure your institutional data is always synchronized
- **Campaign Oversight** — List active and past engagement campaigns and retrieve technical metadata on scheduled nudges
- **Message Auditing** — Retrieve logs of conversational exchanges between students and your AI-powered chatbots
- **Custom Field Mapping** — Manage the metadata used to segment and personalize student interactions across multiple channels
- **Success Monitoring** — Quickly identify student engagement patterns and behavioral trends directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Mainstay API Token
3. Start managing your student engagement and behavioral intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Student Success Officers** — automate the management of student records and monitor engagement health
- **Admissions Teams** — audit prospective student inquiries and track recruitment campaign performance
- **Institutional Researchers** — retrieve behavioral data and message logs for success pattern analysis
- **Enrollment Managers** — manage personalized nudges and student segments using simple natural language commands


## Available Tools (5)
- **list_contacts**: List student contacts
- **get_contact_details**: Get student details
- **list_campaigns**: List engagement campaigns
- **list_messages**: Retrieve message logs
- **list_custom_fields**: List custom metadata fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mainstay (AdmitHub)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a student contact with the name 'Jane Smith'."

**🤖 AI Agent:**
> I've found one student matching 'Jane Smith'. She is currently active in the 'First-Year Orientation' campaign and has replied to 3 nudges this week. Would you like to see her full profile details?

---

**👤 You:**
> "List all active engagement campaigns."

**🤖 AI Agent:**
> I've retrieved your active campaigns. You have 4 live initiatives, including 'Financial Aid Reminders' and 'Campus Housing Nudges'. Would you like to check the message logs for any of them?

---

**👤 You:**
> "Show me the last 10 messages from today."

**🤖 AI Agent:**
> I've retrieved the latest 10 messages. They show active inquiries about registration deadlines and scholarship applications. The AI bot successfully resolved 8 out of 10 requests. Would you like to see the transcripts?


## ❓ FAQ

**Q: Where do I find my Mainstay API Token?**
Log in to the **Mainstay Mascot** application, navigate to the **API Authentication** page. You can generate or retrieve your unique token there. If you don't see this page, contact `support@mainstay.com`.

**Q: Can I see real-time student message logs?**
Yes! Use the `list_messages` tool to retrieve the most recent conversational exchanges between students and the AI bot.

**Q: Does this server support custom field management?**
Yes, you can use the `list_custom_fields` tool to audit the metadata architecture used for personalizing your engagement nudges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mainstay-admithub](https://vinkius.com/mcp/mainstay-admithub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mainstay (AdmitHub)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mainstay-admithub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mainstay (AdmitHub)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mainstay-admithub": {
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
