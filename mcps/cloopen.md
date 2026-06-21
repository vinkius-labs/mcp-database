# Cloopen / 容联云 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloopen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Leading cloud communication platform in China — manage SMS, voice calls, and applications via AI.

## Description
Empower your AI agent to orchestrate your cloud communication with **Cloopen** (容联云), the premier CPaaS provider in China. By connecting Cloopen to your agent, you transform complex SMS campaigns, voice verification, and communication application management into a natural conversation. Your agent can instantly send template-based SMS, initiate voice verification calls, monitor delivery status, and retrieve account information without you ever needing to navigate the comprehensive Cloopen portal. Whether you are automating user verification or coordinating large-scale notifications, your agent acts as a real-time communication assistant, keeping your messages accurate and your delivery reliable.

### What you can do

- **SMS Orchestration** — Send template-based SMS and retrieve real-time delivery status for verification and notifications.
- **Voice Verification** — Initiate automated voice calls to deliver verification codes or critical notifications.
- **Application Management** — List and retrieve detailed information about your communication applications and IVR configs.
- **Account Auditing** — Retrieve high-level account information and monitor your resource usage.
- **Template Control** — Browse approved SMS templates to ensure consistent messaging across your organization.

### How it works

1. Subscribe to this server
2. Enter your Cloopen Account Sid, Auth Token, and App Id
3. Start managing your cloud communication through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Operations** — automate user verification and monitor SMS delivery through natural language queries.
- **Customer Success Teams** — coordinate notifications and manage communication applications directly from your AI-powered workspace.
- **DevOps Engineers** — monitor system communication status and audit account resource usage via a unified AI interface.
- **Cloopen Power Users** — integrate your existing cloud communication workflows into your AI-driven daily routines.


## Available Tools
- **get_account_info**: Get account information
- **get_app**: Get application details
- **get_ivr**: Get IVR configuration
- **list_apps**: List applications
- **list_callback**: Initiate double-call callback
- **list_landing_calls**: Initiate landing call
- **list_templates**: List SMS templates
- **list_voice_codes**: Send voice verification code
- **query_sms**: Query SMS status
- **send_sms**: Send template SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloopen / 容联云** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a verification code '1234' to '13800000000' using template '1'."

**🤖 AI Agent:**
> I've sent the SMS verification code. The message ID is '8821'. You can use this ID to check the delivery status later.

---

**👤 You:**
> "Check my current account balance and info on Cloopen."

**🤖 AI Agent:**
> I've retrieved your account info. You have a balance of ¥500.00 and your account status is 'Active'. Would you like to see your active applications?

---

**👤 You:**
> "List all my approved SMS templates."

**🤖 AI Agent:**
> I've listed your approved SMS templates. You have 3 templates ready for use: 'Verification Code', 'Order Notification', and 'Promotion Alert'. Which one would you like to use?


## ❓ FAQ

**Q: How do I find my Cloopen Account Sid and Token?**
Log in to the Cloopen Console dashboard. You will find your Account Sid and Auth Token in the account information section on the homepage.

**Q: Can I query the status of a specific SMS message?**
Yes. Use the `query_sms` tool with the `smsMessageSid` returned from the send operation to retrieve the current delivery status.

**Q: Is it possible to send voice verification codes?**
Yes! Use the `list_voice_codes` tool to initiate an automated call that will speak the verification code to the recipient's phone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloopen](https://vinkius.com/mcp/cloopen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloopen / 容联云** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cloopen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloopen / 容联云** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloopen": {
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
