# Authkey MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/authkey)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send transactional SMS, voice OTPs, and WhatsApp messages through a unified communication gateway for user verification.

## Description
Connect your **Authkey.io** account to any AI agent and take full control of your multi-channel communication and automated notification workflows through natural conversation.

### What you can do

- **Multichannel Messaging Orchestration** — Instantly dispatch high-fidelity SMS, transactional emails, and voice alerts to customers worldwide using a single unified interface
- **Security & OTP Intelligence** — Programmatically send and verify One-Time Passwords (OTPs) to build secure authentication and 2FA flows directly through your agent
- **Voice Automation Architecture** — Initiate automated voice calls with high-fidelity Text-to-Speech (TTS) or pre-defined templates for critical security alerts
- **Template Management** — Access and monitor your complete directory of communication templates (SMS/Email) to ensure perfectly coordinated brand messaging
- **Financial Visibility Monitoring** — Access real-time balance data across all channels (SMS, Voice, Email) directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Authkey dashboard at authkey.io
3. Start automating your global notifications and engagement from Claude, Cursor, or any MCP client

No more manual toggling between messaging portals or managing multiple protocol integrations. Your AI acts as your dedicated CPaaS engineer and communication coordinator.

### Who is this for?

- **Customer Support Teams** — instantly send order updates and verification codes using natural language commands
- **Security Engineers** — integrate high-speed 2FA and OTP verification into custom bots and internal tools
- **Marketing Leads** — automate the dispatch of omnichannel campaigns and monitor credit usage through simple AI queries


## Available Tools (13)
- **check_balance**: Check balance
- **check_authkey_status**: Verify connectivity
- **get_email_status**: Get email status
- **get_sms_status**: Get SMS status
- **get_voice_status**: Get voice call status
- **list_sms_history**: List SMS history
- **list_templates**: List templates
- **send_bulk_sms**: Send bulk SMS
- **send_email**: Send an email
- **send_otp**: Send OTP
- **send_sms**: Send an SMS
- **send_voice**: Send a voice call
- **verify_otp**: Verify OTP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Authkey** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a security OTP to '+123456789' using template ID '101'."

**🤖 AI Agent:**
> OTP dispatched! I've successfully sent the security code to +123456789. The Log ID for verification is 'auth_992'. Shall I wait for the user to provide the code?

---

**👤 You:**
> "Verify OTP code '5566' for Log ID 'auth_992'."

**🤖 AI Agent:**
> OTP Verified! The code 5566 has been successfully confirmed for the provided session. The high-fidelity identity check is complete. Need any further security actions?

---

**👤 You:**
> "What is my current Authkey account balance across all channels?"

**🤖 AI Agent:**
> Scanning account... Your current balance includes 1,500 SMS credits, 500 Voice minutes, and 10,000 Email credits. You are in good standing for your next notification run. Shall I retrieve your template directory?


## ❓ FAQ

**Q: How do I find my Authkey API Key?**
Log in to your account at [**authkey.io**](https://authkey.io/), navigate to the dashboard, and copy your unique Authkey.

**Q: Can I verify OTPs via AI?**
Yes! The `verify_otp` tool allows your agent to confirm security codes by providing the Log ID from the original request and the code entered by the user.

**Q: How do I check my remaining credits?**
Use the `check_balance` tool to retrieve high-fidelity real-time credit status for SMS, Voice, and Email channels directly through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authkey](https://vinkius.com/mcp/authkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Authkey** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `authkey` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Authkey** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "authkey": {
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
